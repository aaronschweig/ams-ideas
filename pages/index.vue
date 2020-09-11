<template>
  <div class="flex w-screen h-screen">
    <div class="w-1/6 flex px-4 pt-6 flex-col items-start">
      <!-- LOGO AREA -->
      <div
        class="flex items-center w-full p-2 text-text hover:bg-gray-200 rounded-md cursor-pointer hover:shadow transition duration-200"
      >
        <svg
          width="38"
          height="36"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <g filter="url(#filter0_d)">
            <path
              d="M16.997 11.844l4.977 8.647H12.02l4.977-8.647z"
              fill="#1EA9ED"
            />
            <path
              d="M16.997 29.134l-4.977-8.646h9.954l-4.977 8.646z"
              fill="#3ABCF3"
            />
            <path
              d="M21.974 20.49l-4.977-8.646h9.954l-4.977 8.647z"
              fill="#2DACEC"
            />
            <path
              d="M12.02 20.49l-4.976-8.646h9.953L12.02 20.49z"
              fill="#3FB5ED"
            />
            <path
              d="M12.02 3.2l-4.976 8.644H26.95L21.974 3.2H12.02z"
              fill="#63BBE8"
            />
            <path
              d="M7.044 29.122l9.959-.003-9.954-17.275-4.982 8.64 4.977 8.638z"
              fill="#8BD8F1"
            />
            <path
              d="M31.933 20.484l-4.982-8.64-9.954 17.275 9.96.003 4.976-8.638z"
              fill="#5EC0EE"
            />
          </g>
          <defs>
            <filter
              id="filter0_d"
              x="-1"
              y="-2"
              width="40"
              height="40"
              filterUnits="userSpaceOnUse"
              color-interpolation-filters="sRGB"
            >
              <feFlood flood-opacity="0" result="BackgroundImageFix" />
              <feColorMatrix
                in="SourceAlpha"
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
              />
              <feOffset dx="2" dy="2" />
              <feGaussianBlur stdDeviation="2" />
              <feColorMatrix
                values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"
              />
              <feBlend in2="BackgroundImageFix" result="effect1_dropShadow" />
              <feBlend
                in="SourceGraphic"
                in2="effect1_dropShadow"
                result="shape"
              />
            </filter>
          </defs>
        </svg>
        <h1 class="ml-6 text-2xl">AMS-Pro</h1>
      </div>
      <!-- MENU ITEMS -->
      <div class="mt-12 w-full h-full text-text">
        <ul class="h-full flex flex-col">
          <MenuItem>
            <template #icon>
              <svg
                class="w-6 h-6"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M4 5a1 1 0 011-1h14a1 1 0 011 1v2a1 1 0 01-1 1H5a1 1 0 01-1-1V5zM4 13a1 1 0 011-1h6a1 1 0 011 1v6a1 1 0 01-1 1H5a1 1 0 01-1-1v-6zM16 13a1 1 0 011-1h2a1 1 0 011 1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-6z"
                ></path>
              </svg>
            </template>
            Dashbaord
          </MenuItem>
          <MenuItem activated>
            <template #icon>
              <svg
                class="w-6 h-6"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M15 7a2 2 0 012 2m4 0a6 6 0 01-7.743 5.743L11 17H9v2H7v2H4a1 1 0 01-1-1v-2.586a1 1 0 01.293-.707l5.964-5.964A6 6 0 1121 9z"
                ></path>
              </svg>
            </template>
            Betriebsmittel
          </MenuItem>
          <MenuItem>
            <template #icon>
              <svg
                class="w-6 h-6"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M17.657 18.657A8 8 0 016.343 7.343S7 9 9 10c0-2 .5-5 2.986-7C14 5 16.09 5.777 17.656 7.343A7.975 7.975 0 0120 13a7.975 7.975 0 01-2.343 5.657z"
                ></path>
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9.879 16.121A3 3 0 1012.015 11L11 14H9c0 .768.293 1.536.879 2.121z"
                ></path>
              </svg>
            </template>
            Gefahrstoffe
          </MenuItem>
          <MenuItem>
            <template #icon>
              <svg
                class="w-6 h-6"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01"
                ></path>
              </svg>
            </template>
            Gefährdungsbeurteilungen
          </MenuItem>
          <MenuItem>
            <template #icon>
              <svg
                class="w-6 h-6"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"
                ></path>
              </svg>
            </template>
            Betriebsanweisungen
          </MenuItem>
          <MenuItem>
            <template #icon>
              <svg
                class="w-6 h-6"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"
                ></path></svg
            ></template>
            Verbandbuch
          </MenuItem>
          <div class="flex-grow"></div>
          <MenuItem class="mb-8">
            <template #icon>
              <svg
                class="w-6 h-6"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z"
                ></path>
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"
                ></path>
              </svg>
            </template>
            Einstellungen
          </MenuItem>
        </ul>
      </div>
    </div>
    <div
      style="box-shadow: inset 0 8px 16px 0 rgba(0, 0, 0, 0.15)"
      class="w-1/6 bg-secondary"
    >
      <div
        class="flex items-center justify-center text-text border-b border-text border-opacity-25 py-8"
      >
        <button
          class="uppercase flex space-x-2 tracking-tighter focus:outline-none hover:text-highlight rounded-md cursor-pointer transition-colors duration-200"
        >
          <span>Neues Betriebsmittel</span>
          <svg
            class="w-6 h-6"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M12 6v6m0 0v6m0-6h6m-6 0H6"
            ></path>
          </svg>
        </button>
      </div>
      <div class="text-gray-900 pt-6 pl-6">
        <h2 class="text-2xl">Betriebsmittel</h2>
        <div class="space-y-4 mt-8">
          <PresetCard active :count="204">
            Betriebsmittel
            <!---->
          </PresetCard>
          <PresetCard :count="123">
            ohne Mängel
            <!---->
          </PresetCard>
          <PresetCard :count="32">
            mit geringen Mängel
            <!---->
          </PresetCard>
          <PresetCard :count="54">
            mit erheblichen Mängel
            <!---->
          </PresetCard>
        </div>
      </div>
    </div>
    <div class="w-2/3">
      <!-- HEADER BAR -->
      <div
        class="border-b border-text border-opacity-25 text-text flex items-center"
        style="height: 5.5rem"
      >
        <div
          class="ml-8 cursor-pointer rounded-full hover:bg-gray-200 transition duration-200 p-2"
        >
          <svg
            class="w-8 h-8"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
            ></path>
          </svg>
        </div>
        <div class="flex-grow"></div>
        <div class="text-gray-900 flex items-center space-x-2 h-full pr-4">
          <img
            class="inline-block h-8 w-8 rounded-full text-white shadow-md"
            src="https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
            alt=""
          />
          <p class="pl-2">
            Guten Tag, <span class="font-bold">Thomas Schweig</span>!
          </p>
          <div
            class="cursor-pointer rounded-full hover:bg-gray-200 transition duration-200 p-2"
          >
            <svg
              class="w-6 h-6 text-text"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M19 9l-7 7-7-7"
              ></path>
            </svg>
          </div>
        </div>
        <div class="flex items-center space-x-4 mx-4">
          <div
            class="cursor-pointer rounded-full hover:bg-gray-200 transition duration-200 p-2"
          >
            <svg
              class="w-8 h-8 text-highlight"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9"
              ></path>
            </svg>
          </div>
          <div
            class="cursor-pointer rounded-full hover:bg-gray-200 transition duration-200 p-2"
          >
            <svg
              class="w-8 h-8 text-highlight"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M12 9v3m0 0v3m0-3h3m-3 0H9m12 0a9 9 0 11-18 0 9 9 0 0118 0z"
              ></path>
            </svg>
          </div>
        </div>
      </div>
      <!-- TABLE AREA -->
      <div class="overflow-hidden" style="max-height: calc(100vh - 88px)">
        <AmsTable />
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
