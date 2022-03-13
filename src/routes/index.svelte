    <script>
        const toggleTheme = () => {
            let currentTheme = document.documentElement.classList.contains('dark')
            if(currentTheme) {
                document.documentElement.classList.remove('dark')
            }else{
                document.documentElement.classList.add('dark')
            }
            console.log(currentTheme)
        }

    </script>
    <div>
      <span class="inline-flex items-center justify-center p-2 bg-indigo-500 rounded-md shadow-lg">
        <svg class="h-6 w-6 text-white" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true"><!-- ... --></svg>
      </span>
    </div>
    <h3 class="text-slate-900 dark:text-white mt-5 text-base font-medium tracking-tight">Writes Upside-Down</h3>
    <p class="text-slate-500 dark:text-slate-400 mt-2 text-sm">
      The Zero Gravity Pen can be used to write in any orientation, including upside-down. It even works in outer space.
    </p>

    <button class="transition ease-in-out delay-350 hover:bg-indigo-600 bg-indigo-500 text-white text-sm rounded-md px-2 py-1" on:click="{toggleTheme}">Toggle Theme</button>