 <script lang="ts">
  import { Github, Linkedin, Mail } from "lucide-svelte";
</script>

<header
  class="lg:sticky lg:top-0 lg:flex lg:max-h-screen lg:w-1/2 lg:flex-col lg:justify-between lg:py-24"
>
  <div>
    <h1 class="text-4xl font-bold tracking-tight text-slate-200 sm:text-5xl">
      Michel Honoré
    </h1>
    <h2 class="mt-3 text-lg font-medium tracking-tight text-slate-200 sm:text-xl">
      Computer Science Teacher & Software Tinkerer
    </h2>
    <p class="mt-4 max-w-xs leading-normal">
      I teach computer science fundamentals and build software products on the side.
    </p>

    <!-- Navigation -->
    <nav class="nav hidden lg:block" aria-label="In-page jump links">
      <ul class="mt-16 w-max">
        <li>
          <a class="group flex items-center py-3 active" href="#about">
            <span
              class="nav-indicator mr-4 h-px w-8 bg-slate-600 transition-all group-hover:w-16 group-hover:bg-slate-200 group-focus-visible:w-16 group-focus-visible:bg-slate-200 motion-reduce:transition-none"
            ></span>
            <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              About
            </span>
          </a>
        </li>
        <li>
          <a class="group flex items-center py-3" href="#experience">
            <span
              class="nav-indicator mr-4 h-px w-8 bg-slate-600 transition-all group-hover:w-16 group-hover:bg-slate-200 group-focus-visible:w-16 group-focus-visible:bg-slate-200 motion-reduce:transition-none"
            ></span>
            <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Experience
            </span>
          </a>
        </li>
        <li>
          <a class="group flex items-center py-3" href="#projects">
            <span
              class="nav-indicator mr-4 h-px w-8 bg-slate-600 transition-all group-hover:w-16 group-hover:bg-slate-200 group-focus-visible:w-16 group-focus-visible:bg-slate-200 motion-reduce:transition-none"
            ></span>
            <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Projects
            </span>
          </a>
        </li>
      </ul>
    </nav>
    <br>

<!-- Skills -->
    <section class="nav hidden lg:block" aria-label="skillset">
      <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Programming Languages
            </span>
      <ul class="mt-2 flex flex-wrap space-x-1 space-y-1 w-50">
        <li>
            
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Python
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  JavaScript
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Arduino/C++
                </div>
        </li>
        </ul>
        <br>

        <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Frameworks & Tools
            </span>
        <ul class="mt-2 flex flex-wrap space-x-1 space-y-1 w-50">
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Git
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  GitHub
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Streamlit
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Django
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Render
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Railway
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Supabase
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Gemini CLI
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Jules Agent
                </div>
        </li>
        </ul>
        <br>

        <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Education
            </span>
        <ul class="mt-2 flex flex-wrap space-x-1 space-y-1 w-50">
        <li>
            
            <div
                  class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs font-medium leading-5 text-fuchsia-300"
                >
                  CS Principles
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs font-medium leading-5 text-fuchsia-300"
                >
                  Project-based Learning
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs font-medium leading-5 text-fuchsia-300"
                >
                  Robotics
                </div>
        </li>
      </ul>
    </section>
  </div>


  <!-- Social Links -->
  <ul class="ml-1 mt-8 flex items-center" aria-label="Social media">
    <li class="mr-5 text-xs">
      <a
        class="block hover:text-slate-200"
        href="https://github.com/micho8cho93"
        target="_blank"
        rel="noreferrer"
      >
        <Github class="h-6 w-6" />
      </a>
    </li>
    <li class="mr-5 text-xs">
      <a
        class="block hover:text-slate-200"
        href="https://www.linkedin.com/in/michel-honore-95a08549/"
        target="_blank"
        rel="noreferrer"
      >
        <Linkedin class="h-6 w-6" />
      </a>
    </li>
    <li class="mr-5 text-xs">
      <a
        class="block hover:text-slate-200"
        href="mailto:michelvahonore@gmail.com"
        target="_blank"
        rel="noreferrer"
      >
        <Mail class="h-6 w-6" />
      </a>
    </li>
  </ul>
</header>

