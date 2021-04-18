<template>
  <div class="text-gray-900 text-sm">
    <!-- navigation -->
    <nav class="bg-gray-900 text-white px-4 py-3 flex items-center justify-between">

      <!-- left -->
      <div class="flex items-center space-x-4">

        <!-- logo -->
        <a class="text-white hover:text-gray-400" href="#">
          <svg class="w-8 fill-current" viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
        </a>

        <!-- search -->
        <div class="relative">
          <input class="rounded bg-gray-700 placeholder-gray-400 w-72 px-3 py-1" type="text" placeholder="Search or jump to..">
          <div class="absolute top-0 right-0 flex items-center h-full">
            <div class="border border-gray-600 rounded text-xs text-gray-400 px-2 mr-2">/</div>
          </div>
        </div>

        <!-- links -->
        <ul class="flex items-center font-semibold space-x-4">
          <li><a class="hover:text-gray-400" href="#">Pull requests</a></li>
          <li><a class="hover:text-gray-400" href="#">Issues</a></li>
          <li><a class="hover:text-gray-400" href="#">Marketplace</a></li>
          <li><a class="hover:text-gray-400" href="#">Explore</a></li>
        </ul>
      </div>

      <!-- right -->
      <div class="flex items-center space-x-4 text-white">
        <a class="relative hover:text-gray-400" href="#">
          <svg class="w-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"></path></svg>
          <div class="bg-blue-600 rounded-full w-2 h-2 absolute top-0 right-0"></div>
        </a>

        <a class="relative flex items-center hover:text-gray-400" href="#">
          <svg class="w-5" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path></svg>
          <div class="bg-blue-600 rounded-full w-2 h-2 absolute top-0 right-0"></div>
        </a>
      </div>
    </nav>

    <!-- repo namespace / links -->
    <div class="bg-gray-100 border-b border-gray-200 px-4">

      <!-- repo namespace -->
      <div class="flex items-center justify-between">
        <!-- repo namespace links -->
        <div class="text-xl text-blue-600 py-3 flex">
          <svg class="w-5 text-gray-900" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 4v12l-4-2-4 2V4M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z"></path></svg>
          <a class="ml-2" href="#">tailwindlabs</a>
          <span class="mx-1">/</span>
          <a class="font-bold" href="#">tailwindcss</a>
        </div>

        <!-- page actions buttons -->
        <div>
          <!-- watch -->
          <PageActionButton
            text="Watch"
            number="529"
          >
            <svg class="w-4 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z"></path></svg>
          </PageActionButton>

          <!-- star -->
          <PageActionButton
            text="Star"
            number="40.3k"
          >
            <svg class="w-4 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z"></path></svg>
          </PageActionButton>

          <!-- fork -->
          <PageActionButton
            text="Fork"
            number="1.8k"
          >
            <svg class="w-4 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"></path></svg>
          </PageActionButton>


          <!-- <a class="inline-flex items-center bg-transparent border border-gray-400 rounded text-xs" href="#">
            <div class="flex px-2 py-1 border-r border-gray-400 rounded-l">
              <svg class="w-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z"></path></svg>
              <span class="ml-1">Watch</span>
            </div>
            <span class="px-2 py-1 bg-white rounded-r font-bold">529</span>
          </a> -->

          <!-- <a class="px-2 py-1 bg-white border border-gray-400 rounded" href="#">
            <span class="bg-gray-200">Star</span>
            <span class="bg-white">40.3k</span>
          </a>
          <a class="px-2 py-1 bg-white border border-gray-400 rounded" href="#">
            <span class="bg-gray-200">Fork</span>
            <span class="bg-white">1.8k</span>
          </a> -->
        </div>
      </div>

      <!-- links -->
      <div>
        <a class="inline-flex px-4 py-3 font-bold border-b-2 border-yellow-500" href="#">
          <svg class="w-4" viewBox="0 0 16 16"><path fill-rule="evenodd" d="M4.72 3.22a.75.75 0 011.06 1.06L2.06 8l3.72 3.72a.75.75 0 11-1.06 1.06L.47 8.53a.75.75 0 010-1.06l4.25-4.25zm6.56 0a.75.75 0 10-1.06 1.06L13.94 8l-3.72 3.72a.75.75 0 101.06 1.06l4.25-4.25a.75.75 0 000-1.06l-4.25-4.25z"></path></svg>
          <!-- <svg class="w-4" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"></path></svg> -->
          <span class="ml-2">Code</span>
        </a>
        <a class="inline-flex px-4 py-3 " href="#">
          <svg class="w-4 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
          <span class="ml-2">Issues</span>
          <span class="bg-gray-300 rounded-xl px-2 ml-2 text-xs flex items-center">92</span>
        </a>
        <a class="inline-flex px-4 py-3" href="#">
          <svg class="w-4 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4"></path></svg>
          <span class="ml-2">Pull requests</span>
          <span class="bg-gray-300 rounded-xl px-2 ml-2 text-xs flex items-center">35</span>
        </a>
        <a class="inline-flex px-4 py-3" href="#">
          <svg class="w-4 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8h2a2 2 0 012 2v6a2 2 0 01-2 2h-2v4l-4-4H9a1.994 1.994 0 01-1.414-.586m0 0L11 14h4a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2v4l.586-.586z"></path></svg>
          <span class="ml-2">Discussions</span>
        </a>
        <a class="inline-flex px-4 py-3" href="#">
          <svg class="w-4 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
          <span class="ml-2">Actions</span>
        </a>
        <a class="inline-flex px-4 py-3" href="#">
          <svg class="w-4 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.618 5.984A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016zM12 9v2m0 4h.01"></path></svg>
          <span class="ml-2">Security</span>
        </a>
        <a class="inline-flex px-4 py-3" href="#">
          <svg class="w-4 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 12l3-3 3 3 4-4M8 21l4-4 4 4M3 4h18M4 4h16v12a1 1 0 01-1 1H5a1 1 0 01-1-1V4z"></path></svg>
          <span class="ml-2">Insights</span>
        </a>
      </div>

    </div>
  </div>
</template>

<script>
import PageActionButton from './../components/PageActionButton';
export default {
  components: {
    PageActionButton,
  }
}
</script>
