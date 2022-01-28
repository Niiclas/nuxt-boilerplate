<template>
  <div class="card shadow-lg bg-base-100">
    <div class="grid grid-cols-2">
      <div class="card-body grid gap-5 grid-flow-row place-content-stretch">
        <mInput placeholder="Name" label="Wie heißt du" />
        <mInput
          placeholder="Email"
          label="Und wie erreichen wir dich"
          badge="COOL!"
        />
        <mButton primary>Anmelden</mButton>
      </div>
      <div class="card-body bg-primary justify-end">
        <h2 class="text-base-100 text-7xl">Cool, dass du dabei bist!</h2>
      </div>
    </div>
  </div>
</template>
