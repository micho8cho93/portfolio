<script lang="ts">
  import { ExternalLink } from "lucide-svelte";
  let showModal = false;
  let videoURL = "";
</script>

<section
  id="projects"
  class="mb-16 scroll-mt-16 md:mb-24 lg:mb-36 lg:scroll-mt-24"
>
  <div
    class="sticky top-0 z-20 -mx-6 mb-4 w-screen bg-slate-900/75 px-6 py-5 backdrop-blur md:-mx-12 md:px-12 lg:sr-only lg:relative lg:top-auto lg:mx-auto lg:w-full lg:px-0 lg:py-0 lg:opacity-0"
  >
    <h2
      class="text-sm font-bold uppercase tracking-widest text-slate-200 lg:sr-only"
    >
      Projects
    </h2>
  </div>
  <div>
    <ul class="group/list">
      <li class="mb-12">
        <div
          class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50"
        >
          <div
            class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"
          ></div>
          <div class="z-10 sm:order-2 sm:col-span-6">
            <h3>
              <a
                class="inline-flex items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300 group/link text-base"
                href="https://soccersocial.up.railway.app/public/"
                target="_blank"
                rel="noreferrer"
                aria-label="Soccer League Management App (opens in a new tab)"
              >
                <span
                  class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"
                ></span>
                <span>
                  Soccer League Management App
                  <ExternalLink
                    class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px"
                  />
                </span>
              </a>
            </h3>
            <p class="text-slate-400 mt-2 text-sm leading-normal">
              A web app for managing soccer league data. View team standings,
              player statistics, and match schedules. Create and manage teams,
              players, and matches with ease. Built-in administration panel
              for league organizers.
            </p>
            <ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Django
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Tailwind
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Railway
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-purple-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  PostgreSQL
                </div>
              </li>
            </ul>
          </div>
          <img
            alt="Soccer League Management App"
            loading="lazy"
            width="200"
            height="48"
            decoding="async"
            class="rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
            src="/src/public/images/soccer_social1.png"
          />
        </div>
      </li>
      <li class="mb-12">
        <div
          class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50"
        >
          <div
            class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"
          ></div>
          <div class="z-10 sm:order-2 sm:col-span-6">
            <h3>
              <a
                class="inline-flex items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300 group/link text-base"
                href="/src/public/videos/BirthdayBotVideo.mp4"
                target="_blank"
                rel="noreferrer"
                aria-label="Birthday Reminder Bot (opens in a new tab)"
              >
                <span
                  class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"
                ></span>
                <span>
                  Birthday Reminder Bot
                  <ExternalLink
                  on:click={() => {
                showModal = true;
                videoURL = "/src/public/videos/BirthdayBotVideo.mp4";
              }}
                    class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px"
                  />
                </span>
              </a>
            </h3>
            <p class="text-slate-400 mt-2 text-sm leading-normal">
              An automated birthday reminder bot for whatsapp and email. 
              Users can store birthdays and receive reminders via email.
              Each email contains a link that opens Whatsapp Web with your
              pre-written birthday message ready to send. 
            </p>
            <ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Python
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Streamlit
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Render
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Supabase
                </div>
              </li>
            </ul>
          </div>
          <img
            alt="Birthday Reminder Bot"
            loading="lazy"
            width="200"
            height="48"
            decoding="async"
            class="rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
            src="/src/public/images/birthday_bot.png"
          />
        </div>
        {#if showModal}
        <div class="fixed inset-0 z-50 flex items-center justify-center bg-black bg-opacity-50">
          <div class="bg-white rounded-lg p-4">
            <video width="560" height="315" controls autoplay>
              <source src={videoURL} type="video/mp4">
              Your browser does not support the video tag.
            </video>
            <button
              on:click={() => (showModal = false)}
              class="mt-4 bg-teal-300 text-white px-4 py-2 rounded"
              >Close</button
            >
          </div>
        </div>
      {/if}
      </li>
      <li class="mb-12">
        <div
          class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50"
        >
          <div
            class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"
          ></div>
          <div class="z-10 sm:order-2 sm:col-span-6">
            <h3>
              <a
                class="inline-flex items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300 group/link text-base"
                href="https://portfolio-gamma-lyart-95.vercel.app"
                target="_blank"
                rel="noreferrer"
                aria-label="Portfolio v2 (opens in a new tab)"
              >
                <span
                  class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"
                ></span>
                <span>
                  Portfolio v2
                  <ExternalLink
                    class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px"
                  />
                </span>
              </a>
            </h3>
            <p class="text-slate-400 mt-2 text-sm leading-normal">
              Second version of my personal portfolio website.
              Created with a focus on a clean and simple UI/UX design.
              Built using Svelte and Tailwind CSS to familiarize myself 
              with modern web development tools and frameworks.
            </p>
            <ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Sveltekit
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Tailwind CSS
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  GitHub Pages
                </div>
              </li>
            </ul>
          </div>
          <img
            alt="Portfolio v2"
            loading="lazy"
            width="200"
            height="48"
            decoding="async"
            class="rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
            src="/src/public/images/portfoliov2.png"
          />
        </div>
      </li>
      <li class="mb-12">
        <div
          class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50"
        >
          <div
            class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"
          ></div>
          <div class="z-10 sm:order-2 sm:col-span-6">
            <h3>
              <a
                class="inline-flex items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300 group/link text-base"
                href="https://github.com/micho8cho93/Python-Course"
                target="_blank"
                rel="noreferrer"
                aria-label="Python Course (opens in a new tab)"
              >
                <span
                  class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"
                ></span>
                <span>
                  Python Course
                  <ExternalLink
                    class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px"
                  />
                </span>
              </a>
            </h3>
            <p class="text-slate-400 mt-2 text-sm leading-normal">
              An Introduction to Python course designed for High School students.
              The course covers the fundamentals such as variables, statements,
              loops, functions, strings, and lists. Each unit ends with a mini-project
              to apply multiple concepts. The course culminates in a final project 
              where students create a GUI application.
            </p>
            <ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Python
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Github
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Streamlit
                </div>
              </li>
            </ul>
          </div>
          <img
            alt="Python Course"
            loading="lazy"
            width="200"
            height="48" 
            decoding="async"
            class="rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
            src="/src/public/images/python-course.png"
          />
        </div>
      </li>
    </ul>
    <ul>
      <li class="mb-12">
        <div
          class="group relative grid gap-4 pb-1 transition-all sm:grid-cols-8 sm:gap-8 md:gap-4 lg:hover:!opacity-100 lg:group-hover/list:opacity-50"
        >
          <div
            class="absolute -inset-x-4 -inset-y-4 z-0 hidden rounded-md transition motion-reduce:transition-none lg:-inset-x-6 lg:block lg:group-hover:bg-slate-800/50 lg:group-hover:shadow-[inset_0_1px_0_0_rgba(148,163,184,0.1)] lg:group-hover:drop-shadow-lg"
          ></div>
          <div class="z-10 sm:order-2 sm:col-span-6">
            <h3>
              <a
                class="inline-flex items-baseline font-medium leading-tight text-slate-200 hover:text-teal-300 focus-visible:text-teal-300 group/link text-base"
                href="https://micho8cho93.github.io/portfolio.v1/"
                target="_blank"
                rel="noreferrer"
                aria-label="Portfolio v1 (opens in a new tab)"
              >
                <span
                  class="absolute -inset-x-4 -inset-y-2.5 hidden rounded md:-inset-x-6 md:-inset-y-4 lg:block"
                ></span>
                <span>
                  Portfolio v1
                  <ExternalLink
                    class="inline-block h-4 w-4 shrink-0 transition-transform group-hover/link:-translate-y-1 group-hover/link:translate-x-1 group-focus-visible/link:-translate-y-1 group-focus-visible/link:translate-x-1 motion-reduce:transition-none ml-1 translate-y-px"
                  />
                </span>
              </a>
            </h3>
            <p class="text-slate-400 mt-2 text-sm leading-normal">
              The first version of my personal portfolio website.
              Created to showcase my skills and projects.
              Built using HTML, CSS, and JavaScript to learn 
              the basics of web development.
            </p>
            <ul class="mt-2 flex flex-wrap" aria-label="Technologies used">
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  JavaScript
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  CSS
                </div>
              </li>
              <li class="mr-1.5 mt-2">
                <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  HTML
                </div>
              </li>
            </ul>
          </div>
          <img
            alt="Portfolio v1"
            loading="lazy"
            width="200"
            height="48" 
            decoding="async"
            class="rounded border-2 border-slate-200/10 transition group-hover:border-slate-200/30 sm:order-1 sm:col-span-2 sm:translate-y-1"
            src="/src/public/images/portfoliov1.png"
          />
        </div>
      </li>
    </ul>
    <div class="mt-12">
      <a
        class="inline-flex items-center font-medium leading-tight text-slate-200 font-semibold text-slate-200 group"
        aria-label="View Full Project Archive"
        href="/archive"
      >
        <span>
          <span
            class="border-b border-transparent pb-px transition group-hover:border-teal-300 motion-reduce:transition-none"
          >
            View Full Project
          </span>
          <span class="whitespace-nowrap">
            <span
              class="border-b border-transparent pb-px transition group-hover:border-teal-300 motion-reduce:transition-none"
            >
              Archive
            </span>
            <ExternalLink
              class="ml-1 inline-block h-4 w-4 shrink-0 transition-transform group-hover:-translate-y-1 group-hover:translate-x-1 group-focus-visible:-translate-y-1 group-focus-visible:translate-x-1 motion-reduce:transition-none"
            />
          </span>
        </span>
      </a>
    </div>
  </div>
</section>
