<template>
  <div>
    <div class="grid gap-5 grid-cols-1">
      <slot />
      <div class="grid grid-flow-col auto-cols-auto place-content-between">
        <mButton>Abbrechen</mButton>
        <mButton primary>Anwenden</mButton>
      </div>
    </div>
  </div>
</template>
