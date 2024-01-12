<template>
    <div class="navbar-alert">
      <img
        loading="lazy"
        src="../assets/images/logo.svg"
        class="logo"
      />
      <span class="navbar-alert__text">
        <div class="navbar-alert__date">
          <span
            style="
              font-family: Graphik LC, -apple-system, Roboto, Helvetica,
                sans-serif;
              font-weight: 600;
            ">
            Black Friday
          </span>
          <span
            class="tablet_not_visible"
            style="
              font-family: Graphik LC, -apple-system, Roboto, Helvetica,
              sans-serif;
            ">
            , 24-27 Nov
          </span>
        </div>
        <span class="navbar-alert__dot mobile_not_visible">·</span>
        <span class="navbar-alert__percent">
          10%OFF
        </span>
        <span class="navbar-alert__dot mobile_not_visible">·</span>
        <span class="navbar-alert__code mobile_not_visible">
          <span
            style="
              font-family: Graphik LC, -apple-system, Roboto, Helvetica, sans-serif;
              color: #fefefe;
              font-weight: 300;
            ">
            Use code
          </span>
          <span
            style="
              font-family: Graphik LC, -apple-system, Roboto, Helvetica,
                sans-serif;
              font-weight: 600;
              margin: 0 5px;
              color: rgba(215, 168, 48, 1);
            ">
            10FRIDAY
          </span>
          <span
            class="tablet_not_visible"
            style="
              font-family: Graphik LC, -apple-system, Roboto, Helvetica,
                sans-serif;
            ">
            at checkout
          </span>
        </span>
      </span>
      <div class="navbar-alert__actions">
        <span class="navbar-alert__shop-now mobile_not_visible" style="cursor: pointer;">Shop now</span>
        <img
          loading="lazy"
          src="../assets/images/close_icon.svg"
          style="cursor: pointer;"
          class="navbar-alert__icon tablet_not_visible"
        />
        <img
          class="navbar-alert__icon mobile_visible_only"
          loading="lazy"
          style="cursor: pointer;"
          src="../assets/images/menu-icon.svg"
          alt=""
        >
      </div>
    </div>
</template>