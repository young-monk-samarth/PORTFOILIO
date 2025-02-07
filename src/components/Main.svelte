<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "Portfolio",
            icon: "fa-regular fa-address-card",
            description:
                "Smoljames Store is a a merchanising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.",
        },
        {
            name: "Weather App",
            icon:"fa-sharp fa-regular fa-sun",
            description:
                "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
        },
        {
            name: "VideoSummarization",
            icon: "fa-sharp fa-solid fa-video" ,
            description:
                "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "a self taught developer",
            description:
                "I taught myself to code using free online resources and absolutely fell in love with the creativity and problem solving that is involved in developing and engineering innovative new online experiences. Starting of with JavaScript, HTML & CSS and evolving my knowledge base to include JavaScript frameworks, backend programming, design, cloud services and much much more.",
        },
        {
            name: "adaptable & resilient",
            description:
                "An adaptable, resilient, and eager-to-learn individual with a passion for frontend development. Quick to adjust to evolving technologies and challenges, embracing continuous learning to refine skills and stay up with trends. Driven to incorporate design aesthetics into functional, user-centered interfaces."
        },
        {
            name: "a good communicator",
            description:
                "I believe in transparency and constructive communication above all else. I focus on understanding ideas and perspectives, working collaboratively to refine and develop them. This approach helps me build meaningful relationships and enhances productivity and effectiveness within any team or work environment.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">


    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">SAMARTH</span>MUKTAMATH <br>as
                <br />Front End 
                <span class="poppins text-violet-400">Developer</span>
            </h2>

            <p class="font-['Inter'] text-justify text-lg sm:text-xl md:text-2xl leading-relaxed max-w-3xl mx-auto">
                <span class="text-transparent bg-gradient-to-r from-transparent via-violet-100 to-transparent bg-[length:300%_100%] bg-clip-text animate-infinite-reveal font-medium tracking-wide transition-all duration-500 ease-[cubic-bezier(0.4,0,0.2,1)] hover:scale-[1.02] hover:via-blue-400 inline-block">
                    <b class="font-semibold">Information Science Engineering</b> student based in 
                    <span class="underline decoration-wavy decoration-1">Bengaluru</span> with a passion for 
                    <span class="italic"><b class="font-bold violet-400">Web development.</b>
                    </span></span>
            </p>

            <style>
            @keyframes infinite-reveal {
                0% { background-position: 200% 0; }
                100% { background-position: -200% 0; }
            }
            .animate-infinite-reveal {
                animation: infinite-reveal 6s linear infinite;
            }
            </style>

            <!-- get in tch bttn  -->
            <a href="mailto:samarthmise2025@gmail.com" 
            class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 inline-block transition-all duration-300 border-0 outline-none hover:border-0 focus:border-0 active:border-0 hover:outline-none focus:outline-none active:outline-none">
            
             <!-- Black  -->
             <div class="absolute top-0 -left-full w-full h-full bg-black opacity-0 group-hover:opacity-100 group-hover:translate-x-full transition-all duration-300 ease-out"></div>
             
             <!-- Text -->
             <h4 class="relative z-10 transition-colors duration-200 group-hover:text-violet-400">
                 Get in touch &rarr;
             </h4>
         </a>
        </div>

            <!-- photo disply-->
            <div class="wrapper"> <!-- Optional sizing wrapper -->
                <div class="box">
                    <img 
                        src="webpic.jpg" 
                        alt="Zetane Interface"
                        loading="lazy"
                    />
                </div>
            </div>
            
            <style>
            .wrapper {
                width: 400px;  /* Original container size */
                height: 400px;
                margin: 0 auto;
            }
            
            .box {
                position: relative;
                width: 100%;    /* Half width */
                height: 100%;   /* Half height */
                overflow: hidden;
                border-radius:10px 50px 10px 50px;
            }
            
            .box img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                transition: all 1s ease;
            }
            
            .box:hover img {
                transform: scale(1.2);
            }
            </style>
  </section>
       

    <!-- scroll info about creative -->
      <section class="py-16 lg:py-24 flex flex-col gap-16" id="projects">
            <div class="flex flex-col gap-1.5 text-center">
                <h6 class="text-large sm:text-xl md:text-2xl">
                    A few of my creative endeavors.
                </h6>
                <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                    Curious to <span class="poppins text-violet-400">see</span> my work?
                </h3>
            </div>

            <!-- buttn to direct video link -->
            <a
                href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
                target="_blank"
                class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
            >
                <i class="fa-regular fa-circle-play" />
                <p>Watch the video</p>
            </a>

        <!-- Listing  steps    -->

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10 justify-centre">
                <Step step={steps[0]}>
                    <p>
                        My Web Portfolio is a dynamic and interactive website built using <strong
                            class="text-violet-400">  
                            SvelteKit , JavaScript </strong> styled with <strong
                            class="text-violet-400">   TailwindCSS .</strong
                        >  Features dynamic design, smooth transitions,ensuring an optimized user experience while showcasing my expertise in frontend development technologies .
                    </p>
                </Step>
                <Step step={steps[1]}>
                
                    <!-- weatehr desc  -->
                </Step>
                <Step step={steps[2]}>
                    <p>
                        Video Summarization leverages long-duration videos to quickly summarize key content based on user queries, saving significant time. Built with <strong class="text-violet-400">Python</strong> for backend processing, it integrates <strong class="text-violet-400">YOLO (You Only Look Once)</strong> for real-time object detection, while the frontend is designed using <strong class="text-violet-400">CSS</strong> for an intuitive and responsive user interface.
                    </p>
                    
                </Step>
            </div>
        </section>
 





    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>



        
        <section id="tech" class="py-14 sm:py-20">
            <div class="container mx-auto px-4">
                <div class="max-w-6xl mx-auto">
                    <div class="text-center mb-12 lg:mb-16">
                        <h2 class="text-3xl sm:text-4xl md:text-5xl font-semibold">
                            My <span class="poppins text-violet-400">Tech Stack</span>
                        </h2>
                        <p class="text-slate-300 mt-4 text-lg sm:text-xl">
                            Tools & technologies I use to bring ideas to life
                        </p>
                    </div>
        
                    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-4 sm:gap-6">
                        <!-- Tech Items - Updated Hover Effect -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <!-- Glass Background -->
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <!-- Hover Overlay -->
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">◆</span>
                                <h3 class="poppins font-medium text-lg">HTML5</h3>
                                <p class="text-slate-400 text-sm mt-1">Semantic Web</p>
                            </div>
                        </div>
        
                        <!-- CSS3 -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">✦</span>
                                <h3 class="poppins font-medium text-lg">CSS3</h3>
                                <p class="text-slate-400 text-sm mt-1">Styling Master</p>
                            </div>
                        </div>
        
                        <!-- Tailwind -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">❖</span>
                                <h3 class="poppins font-medium text-lg">Tailwind</h3>
                                <p class="text-slate-400 text-sm mt-1">Utility First</p>
                            </div>
                        </div>
        
                        <!-- JavaScript -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">⎇</span>
                                <h3 class="poppins font-medium text-lg">JavaScript</h3>
                                <p class="text-slate-400 text-sm mt-1">ES6+</p>
                            </div>
                        </div>
        
                        <!-- TypeScript -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">Τ</span>
                                <h3 class="poppins font-medium text-lg">TypeScript</h3>
                                <p class="text-slate-400 text-sm mt-1">Typed JS</p>
                            </div>
                        </div>
        
                        <!-- Svelte -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">⚡</span>
                                <h3 class="poppins font-medium text-lg">Svelte</h3>
                                <p class="text-slate-400 text-sm mt-1">Reactive</p>
                            </div>
                        </div>
        
                        <!-- SvelteKit -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">🚀</span>
                                <h3 class="poppins font-medium text-lg">SvelteKit</h3>
                                <p class="text-slate-400 text-sm mt-1">Fullstack</p>
                            </div>
                        </div>
        
                        <!-- C -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2"></span>
                                <h3 class="poppins font-medium text-lg">C</h3>
                                <p class="text-slate-400 text-sm mt-1">System Basics</p>
                            </div>
                        </div>
        
                        <!-- C++ -->
                        <div class="group relative p-4 sm:p-5 rounded-xl border border-slate-700/20 hover:border-violet-400/30 transition-all duration-300 hover:-translate-y-1.5 overflow-hidden">
                            <div class="absolute inset-0 bg-slate-800/20 backdrop-blur-md"></div>
                            <div class="absolute inset-0 bg-violet-600/0 group-hover:bg-violet-600/20 transition-colors duration-300"></div>
                            <div class="relative flex flex-col items-center">
                                <span class="text-violet-400 text-2xl mb-2">++</span>
                                <h3 class="poppins font-medium text-lg">C++</h3>
                                <p class="text-slate-400 text-sm mt-1">OOP</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
        




        
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
          <div class="flex flex-col gap-6 max-w-[800px] mx-auto w-full overflow-x-auto sm:overflow-x-hidden">
        <div class="w-full overflow-x-auto">
            <table class="bg-[#EEE8FD] text-slate-900 rounded-md text-center w-full min-w-[600px]">
                <thead class="border-b border-solid border-slate-200">
                    <tr>
                        <th></th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th class="bg-violet-600 text-white whitespace-nowrap p-4 px-8">Me</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Teamwork & Collaboration</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Resilience & Adaptability</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr>
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Creativity</td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Programming Ability</td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm">Interpersonal Skills</td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
    <div class="mx-auto -mt-8 italic sm:hidden opacity-50 text-center text-sm">
        <p>Scroll to see more &rarr;</p>
    </div>
    <p class="mx-auto text-2xl font-bold font-roboto text-center mt-4">So why not invest?</p>
</section>
</main>
    
