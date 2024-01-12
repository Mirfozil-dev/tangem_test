<template>
    <div class="card-alert">
      <img
        loading="lazy"
        style="z-index: 999; cursor: pointer;"
        src="../assets/images/close_icon.svg"
      />
      <img
        loading="lazy"
        src="../assets/images/card_bg.svg"
        class="card-alert__bg"
      />
      <div class="card-alert__content">
        <div class="card-alert__title">Black Friday</div>
        <div class="card-alert__percent">10%OFF</div>
        <div class="card-alert__code">
          Use code <span style="color: rgba(215, 168, 48, 1)">10FRIDAY</span> at checkout
        </div>
        <span class="card-alert__shop-now" style="cursor: pointer;">Shop now <span class="mobile_not_visible">through Monday</span></span>
      </div>
    </div>
</template>