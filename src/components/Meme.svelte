<script lang="ts">
    import { onMount } from "svelte";
    interface MemeData {
        img: string;
        title: string;
        year: string;
        month: string;
        day: string;
    }

    let img_description : {name?: string, joke?: string, imgdate?: string, isHidden?: boolean} = {}

    onMount(async () => {
        const params = new URLSearchParams({
            email: "e.semenova@innopolis.university"
        });

        const response = await fetch(`https://fwd.innopolis.app/api/hw2?${params.toString()}`);
        const number = await response.text();
        const jokeResponse = await fetch(`https://getxkcd.vercel.app/api/comic?num=${number}`);
        const joke_info: MemeData = await jokeResponse.json();

        img_description = {
            name: `${joke_info.title} `,
            imgdate: `${joke_info.day}.${joke_info.month}.${joke_info.year}`,
            joke: joke_info.img,
            isHidden: false
        }

    })
</script>

<br>
<div class="jokeImg">
    <h4><b> - {img_description.name} - </b></h4>
    <img src={img_description.joke} alt={img_description.imgdate} hidden={img_description.isHidden}>
    <figure>
        <h5>Date: {img_description.imgdate}</h5>
    </figure>
</div>
<style>

</style>