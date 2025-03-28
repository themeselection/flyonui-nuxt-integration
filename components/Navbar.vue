<template>
  <nav class="navbar shadow">
    <div class="navbar-start">
      <NuxtLink
        class="link text-base-content/90 link-neutral text-xl font-semibold no-underline"
        to="/"
      >
        FlyonUI
      </NuxtLink>
    </div>
    <div class="navbar-center max-sm:hidden">
      <ul class="menu menu-horizontal gap-2 p-0 text-base rtl:ml-20">
        <li
          class="dropdown relative inline-flex [--offset:9] [--placement:bottom-end] max-sm:[--placement:bottom]"
        >
          <button
            id="dropdown-css-components"
            type="button"
            class="dropdown-toggle dropdown-open:bg-base-content/10 dropdown-open:text-base-content max-sm:px-2"
            aria-haspopup="menu"
            aria-expanded="false"
            aria-label="Dropdown"
          >
            CSS Components
            <span
              class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4"
            ></span>
          </button>
          <ul
            class="dropdown-menu dropdown-open:opacity-100 hidden"
            role="menu"
            aria-orientation="vertical"
            aria-labelledby="ui-components"
          >
            <li>
              <NuxtLink class="dropdown-item" to="/button">Button</NuxtLink>
            </li>
            <li>
              <NuxtLink class="dropdown-item" to="/card">Card</NuxtLink>
            </li>
            <li>
              <NuxtLink class="dropdown-item" to="/form-elements"
                >Form Elements</NuxtLink
              >
            </li>
          </ul>
        </li>
        <li
          class="dropdown relative [--offset:9] [--placement:bottom-end] max-sm:[--placement:bottom]"
        >
          <button
            id="dropdown-js-components"
            class="dropdown-toggle dropdown-item dropdown-open:bg-base-content/10 dropdown-open:text-base-content justify-between"
            aria-haspopup="menu"
            aria-expanded="false"
            aria-label="Dropdown"
          >
            JS Components
            <span
              class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-4 rtl:rotate-180"
            ></span>
          </button>
          <ul
            class="dropdown-menu dropdown-open:opacity-100 hidden"
            role="menu"
            aria-orientation="vertical"
            aria-labelledby="js-components"
          >
            <li>
              <NuxtLink class="dropdown-item" to="/accordion"
                >Accordion</NuxtLink
              >
            </li>
            <li>
              <NuxtLink class="dropdown-item" to="/overlays">Overlays</NuxtLink>
            </li>
            <li>
              <NuxtLink class="dropdown-item" to="/advance-forms"
                >Advance Forms</NuxtLink
              >
            </li>
          </ul>
        </li>
      </ul>
    </div>
    <div class="navbar-end items-center gap-4">
      <div
        class="dropdown relative inline-flex sm:hidden rtl:[--placement:bottom-end]"
      >
        <button
          id="dropdown-default"
          type="button"
          class="dropdown-toggle btn btn-outline btn-secondary btn-square"
          aria-haspopup="menu"
          aria-expanded="false"
          aria-label="Dropdown"
        >
          <span
            class="icon-[tabler--menu-2] dropdown-open:hidden size-5"
          ></span>
          <span
            class="icon-[tabler--x] dropdown-open:block hidden size-5"
          ></span>
        </button>
        <ul
          class="dropdown-menu dropdown-open:opacity-100 hidden min-w-60"
          role="menu"
          aria-orientation="vertical"
          aria-labelledby="dropdown-default"
        >
          <li
            class="dropdown relative [--offset:9] [--placement:bottom-end] max-sm:[--placement:bottom]"
          >
            <button
              id="dropdown-css-components-2"
              class="dropdown-toggle dropdown-item dropdown-open:bg-base-content/10 dropdown-open:text-base-content justify-between"
              aria-haspopup="menu"
              aria-expanded="false"
              aria-label="Dropdown"
            >
              CSS Components
              <span
                class="icon-[tabler--chevron-right] size-4 rtl:rotate-180"
              ></span>
            </button>
            <ul
              class="dropdown-menu dropdown-open:opacity-100 hidden"
              role="menu"
              aria-orientation="vertical"
              aria-labelledby="ui-components"
            >
              <NuxtLink to="/button"
                ><li><a class="dropdown-item">Button</a></li></NuxtLink
              >
              <NuxtLink to="/card"
                ><li><a class="dropdown-item">Card</a></li></NuxtLink
              >
              <NuxtLink to="/form-elements"
                ><li><a class="dropdown-item">Form Elements</a></li></NuxtLink
              >
            </ul>
          </li>
          <li
            class="dropdown relative [--offset:9] [--placement:bottom-end] max-sm:[--placement:bottom]"
          >
            <button
              id="dropdown-js-components-2"
              class="dropdown-toggle dropdown-item dropdown-open:bg-base-content/10 dropdown-open:text-base-content justify-between"
              aria-haspopup="menu"
              aria-expanded="false"
              aria-label="Dropdown"
            >
              JS Components
              <span
                class="icon-[tabler--chevron-right] size-4 rtl:rotate-180"
              ></span>
            </button>
            <ul
              class="dropdown-menu dropdown-open:opacity-100 hidden"
              role="menu"
              aria-orientation="vertical"
              aria-labelledby="js-components"
            >
              <NuxtLink to="/accordion"
                ><li><a class="dropdown-item">Accordion</a></li></NuxtLink
              >
              <NuxtLink to="/overlays"
                ><li><a class="dropdown-item">Overlays</a></li></NuxtLink
              >
              <NuxtLink to="/advance-forms"
                ><li><a class="dropdown-item">Advance Forms</a></li></NuxtLink
              >
            </ul>
          </li>
        </ul>
      </div>
      <div class="dropdown relative inline-flex rtl:[--placement:bottom-end]">
        <button
          id="dropdown-default"
          type="button"
          class="dropdown-toggle btn btn-primary btn-outline max-sm:btn-square"
          aria-haspopup="menu"
          aria-expanded="false"
          aria-label="Dropdown"
        >
          <span class="max-sm:hidden">Theme</span>
          <span class="icon-[tabler--aperture] block size-6 sm:hidden"></span>
          <span
            class="icon-[tabler--chevron-down] dropdown-open:rotate-180 size-5 max-sm:hidden"
          ></span>
        </button>
        <ul
          class="dropdown-menu dropdown-open:opacity-100 hidden min-w-40"
          role="menu"
          aria-orientation="vertical"
          aria-labelledby="dropdown-default"
        >
          <li>
            <input
              type="radio"
              name="theme-dropdown"
              class="theme-controller btn btn-text w-full justify-start"
              aria-label="Default"
              value="default"
              defaultChecked
            />
          </li>
          <li>
            <input
              type="radio"
              name="theme-dropdown"
              class="theme-controller btn btn-text w-full justify-start"
              aria-label="Dark"
              value="dark"
            />
          </li>
          <li>
            <input
              type="radio"
              name="theme-dropdown"
              class="theme-controller btn btn-text w-full justify-start"
              aria-label="Gourmet"
              value="gourmet"
            />
          </li>
          <li>
            <input
              type="radio"
              name="theme-dropdown"
              class="theme-controller btn btn-text w-full justify-start"
              aria-label="Corporate"
              value="corporate"
            />
          </li>
          <li>
            <input
              type="radio"
              name="theme-dropdown"
              class="theme-controller btn btn-text w-full justify-start"
              aria-label="Luxury"
              value="luxury"
            />
          </li>
          <li>
            <input
              type="radio"
              name="theme-dropdown"
              class="theme-controller btn btn-text w-full justify-start"
              aria-label="Soft"
              value="soft"
            />
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>
