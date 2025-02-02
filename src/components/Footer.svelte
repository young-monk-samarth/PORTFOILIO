<footer
    class="py-20 sm:py-32 bg-black border-t border-solid border-violet-950 flex flex-col gap-4 sm:gap-8 justify-center items-center"
>
<div class="pure-scroller">
    <div class="scroller-track">
      <span class="scroll-text">OPEN TO WORK  </span>
      <span class="scroll-text">LOOKING FOR INTERNSHIP  </span>
      <span class="scroll-text">OPEN TO WORK  </span>
      <span class="scroll-text">LOOKING FOR INTERNSHIP  </span>

    </div>
  </div>
  
  <style>
  :root {
    --text-color: white;
    --scroll-speed: 15s;
    --text-size: 1.5rem;
  }
  


  .pure-scroller {
position:bottom center;
overflow:hidden;
top: 100px; /* Adjust based on header height */
width: 100%;
left: 0;
right: 0;
z-index: 100;
background: #080808; /* Semi-transparent background */
color: white !important; /* Text color */
}    
  .scroller-track {
    display: inline-flex;
    animation: scroll var(--scroll-speed) linear infinite;
    white-space: nowrap;
  }
  
  .scroll-text {
    display: inline-flex;
    align-items: center;
    color: var(--text-color);
    font-size: var(--text-size);
    font-weight: 800;
    text-transform: uppercase;
    letter-spacing: 3px;
    padding: 0 2rem;
    position: relative;
    text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
  }
  
  .scroll-text::after {
    content: "\f08c""\f061";
    font-family: FontAwesome;
    margin: 0 3rem;
    opacity: 0.7;
    font-size:1rem;
  }
  
  @keyframes scroll {
    0% { transform: translateX(100%); }
    100% { transform: translateX(-100%); }
  }
  
  /* Dynamic underline animation */
  .scroll-text:hover {
    animation: text-glow 1.2s ease-in-out infinite;
  }
  
  @keyframes text-glow {
    0%, 100% { 
      text-shadow: 0 0 10px rgba(0,0,0,0.1),
                   0 0 20px rgba(0,0,0,0.1);
    }
    50% { 
      text-shadow: 0 0 15px rgba(0,0,0,0.2),
                   0 0 25px rgba(0,0,0,0.2);
    }
  }
  
  /* Mobile Optimization */
  @media (max-width: 768px) {
    :root {
      --text-size: 1.8rem;
    }
    .scroll-text::after {
      margin: 0 1rem;
    }
  }
  </style>






<p 
    class="px-6 py-1 bg-white text-slate-950 font-medium rounded-md transition-all duration-200 hover:bg-black group relative cursor-pointer text-lg" 
    id="connect"
>
    <span class="inline-block group-hover:text-white transition-colors duration-200 align-middle">
        Connect with me 
        <span class="inline-block text-2xl ml-1 animate-[bounce-fast_0.5s_infinite]">
            &darr;
        </span>
    </span>
</p>

<style>
    @keyframes bounce-fast {
        0%, 100% { transform: translateY(0); }
        50% { transform: translateY(-6px); }
    }
    .animate-\[bounce-fast_0\.5s_infinite\] {
        animation: bounce-fast 0.5s infinite;
    }
</style>    


    <!-- gmail icon -->
    <div class="flex flex-col gap-4 items-center justify-center">
        <p class="flex items-center gap-2">
            <svg 
                xmlns="http://www.w3.org/2000/svg" 
                width="24" 
                height="24" 
                viewBox="0 0 64 64"
                class="w-5 h-5 text-gray-100 fill-current"
            >
                <path d="M55,10H9c-2.209,0-4,1.791-4,4v34c0,2.209,1.791,4,4,4h46c2.209,0,4-1.791,4-4V14C59,11.791,57.209,10,55,10z M55,45.738 C54.954,47,53.901,48,52.618,48H49.5L51,21L32,33L13,22l1.5,26h-3.118C10.099,48,9.046,47,9,45.738V16.289 c0-1.25,1.03-2.263,2.3-2.263h1.2L32,29l19.5-14.974h1.2c1.27,0,2.3,1.013,2.3,2.263V45.738z"></path>
            </svg>
            <b class="pr-2">Email</b>
            <a 
                href="mailto:samarthmise2025@gmail.com" 
                class="text-violet-400 hover:text-violet-300 transition-colors"
            >
                samarthmise2025@gmail.com
            </a>
        </p>

        <!-- github icon -->
        <p class="flex items-center gap-2">
            <svg 
                xmlns="http://www.w3.org/2000/svg" 
                width="34" 
                height="34" 
                viewBox="0 0 64 64"
                class="w-5 h-5 text-gray-100 fill-current"
            >
                <path d="M32 6C17.641 6 6 17.641 6 32c0 12.277 8.512 22.56 19.955 25.286-.592-.141-1.179-.299-1.755-.479V50.85c0 0-.975.325-2.275.325-3.637 0-5.148-3.245-5.525-4.875-.229-.993-.827-1.934-1.469-2.509-.767-.684-1.126-.686-1.131-.92-.01-.491.658-.471.975-.471 1.625 0 2.857 1.729 3.429 2.623 1.417 2.207 2.938 2.577 3.721 2.577.975 0 1.817-.146 2.397-.426.268-1.888 1.108-3.57 2.478-4.774-6.097-1.219-10.4-4.716-10.4-10.4 0-2.928 1.175-5.619 3.133-7.792C19.333 23.641 19 22.494 19 20.625c0-1.235.086-2.751.65-4.225 0 0 3.708.026 7.205 3.338C28.469 19.268 30.196 19 32 19s3.531.268 5.145.738c3.497-3.312 7.205-3.338 7.205-3.338.567 1.474.65 2.99.65 4.225 0 2.015-.268 3.19-.432 3.697C46.466 26.475 47.6 29.124 47.6 32c0 5.684-4.303 9.181-10.4 10.4 1.628 1.43 2.6 3.513 2.6 5.85v8.557c-.576.181-1.162.338-1.755.479C49.488 54.56 58 44.277 58 32 58 17.641 46.359 6 32 6zM33.813 57.93C33.214 57.972 32.61 58 32 58 32.61 58 33.213 57.971 33.813 57.93zM37.786 57.346c-1.164.265-2.357.451-3.575.554C35.429 57.797 36.622 57.61 37.786 57.346zM32 58c-.61 0-1.214-.028-1.813-.07C30.787 57.971 31.39 58 32 58zM29.788 57.9c-1.217-.103-2.411-.289-3.574-.554C27.378 57.61 28.571 57.797 29.788 57.9z"></path>
            </svg>
            <b class="pr-2">GitHub</b>
            <a 
                href="https://github.com/young-monk-samarth?tab=repositories" 
                target="_blank" 
                class="text-violet-400 hover:text-violet-300 transition-colors"
            >
                SAMARTH MUKTAMATH
                <sup>
                    <span class="text-xs scale-75 pl-0.5">
                        <i class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"></i>
                    </span>
                </sup>
            </a>
        </p>

        <!-- linkedin logo -->
        <p class="flex items-center gap-2">
            <svg 
                xmlns="http://www.w3.org/2000/svg" 
                width="34" 
                height="34" 
                viewBox="0 0 50 50"
                class="w-5 h-5 text-gray-100 fill-current"
            >
                <path d="M41,4H9C6.24,4,4,6.24,4,9v32c0,2.76,2.24,5,5,5h32c2.76,0,5-2.24,5-5V9C46,6.24,43.76,4,41,4z M17,20v19h-6V20H17z M11,14.47c0-1.4,1.2-2.47,3-2.47s2.93,1.07,3,2.47c0,1.4-1.12,2.53-3,2.53C12.2,17,11,15.87,11,14.47z M39,39h-6c0,0,0-9.26,0-10 c0-2-1-4-3.5-4.04h-0.08C27,24.96,26,27.02,26,29c0,0.91,0,10,0,10h-6V20h6v2.56c0,0,1.93-2.56,5.81-2.56 c3.97,0,7.19,2.73,7.19,8.26V39z"></path>
            </svg>
            <b class="pr-2">LinkedIn</b>
            <a 
                href="https://www.linkedin.com/in/samarthmuktamath?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" 
                target="_blank" 
                class="text-violet-400 hover:text-violet-300 transition-colors"
            >
                SAMARTH MUKTAMATH
                <sup>
                    <span class="text-xs scale-75 pl-0.5">
                        <i class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"></i>
                    </span>
                </sup>
            </a>
        </p>



    </div>
</footer>
 