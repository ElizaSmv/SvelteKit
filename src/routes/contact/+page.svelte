<script>
    import {base} from "$app/paths";
</script>

<h1> * My contacts * </h1><br>
<h4>You can contact me via Telegram or using my phone number.</h4><br>
<ul style="margin-block-start: 0;">
    <li><a href="https://t.me/eliza_smv" id="tg-link">
        <img src ="{base}/lib/images/telegram-logo.jpg" height="40px" alt="telegram"/></a> Telegram  .</li>
    <li><a href="https://instagram.com/eliza_smv/" id="insta-link">
        <img src ="{base}/lib/images/inst.png" height="40px" alt="insta"/></a> Instagram  .</li>
    <li><a href="https://github.com/ElizaSmv" id="github-link">
        <img src ="{base}/lib/images/github.png" height="40px" alt="git"/></a> Github  .</li>
</ul>
<p></p>
<p><img src ="{base}/lib/images/phone.jpg" height="40px" alt="phone number"/>
    My phone number: <a href="tel:+79774984921">8-977-498-49-21</a> </p>
<p></p>

<div class="container">
    <form>
        <h2> GET IN TOUCH </h2>
        <input type="text" id="name" placeholder="Enter Your Name" required>
        <input type="email" id="email" placeholder="Enter Your Email" required>

        <textarea id="message" rows="4" placeholder="Write Something"></textarea>
        <button type="submit">Send</button>
    </form>
</div>

<style>
    .container {
        background-color: #ebe6ea;
        /*display: flex;*/
        align-items: center;
        padding: 20px;
        height: 100vh;
    }

    form {
        background-color: #ddabfa;
        display: flex;
        flex-direction: column;
        padding: 2vw 4vw;
        width: 60%;
        max-width: 500px;
        border-radius: 10px;
    }

    form h2 {
        text-align: center;
        color: #403d58;
        margin-bottom: 20px;
    }

    form input, textarea {
        border: 0;
        margin: 10px 0;
        padding: 20px;
        outline: none;
        background: #eef1f6;
        font-size: 16px;
        border-radius: 10px;
        resize: none;
    }

    form button {
        background: #ebe6ea;
        color: #403d58;
        border: 1px solid #403d58;
        padding: 15px;
        font-size: 1rem;
        outline: none;
        cursor: pointer;
        width: 100%;
        font-weight: bold;
        margin: 20px auto 0;
        border-radius: 30px;
        transition: all .5s ease-in;
    }

    form button:hover {
        border: 1px solid #403d58;
        background: #403d58;
        color: white;
    }
</style>