<template>
  <v-card
    class="mx-auto"
    max-width="344"
    elevation="24"
    outlined
    shaped
    id="cards"
  >
    <v-card-text id="cards">
      <!-- <div>Word of the Day</div> -->
      <p class="text-h4">
        {{ CardData.Name }}
      </p>

      <p text color="teal accent-4" style="font-weight: bold; font-size: large">
        {{ CardData.Centre }}
      </p>
      <div class="">
        {{ CardData.Designation }}
      </div>
    </v-card-text>
    <v-card-actions>
      <!-- <p text color="teal accent-4" @click="reveal = true"> -->
      <p>{{ CardData.Department }}</p>
    </v-card-actions>

    <!-- <v-expand-transition>
            <v-card v-if="reveal" class="transition-fast-in-fast-out v-card--reveal" style="height: 100%;">
                <v-card-text class="pb-0">
                    <p class="text-h4 text--primary">
                        Origin
                    </p>
                    <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin
                        eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
                </v-card-text>
                <v-card-actions class="pt-0">
                    <v-btn text color="teal accent-4" @click="reveal = false">
                        Close
                    </v-btn>
                </v-card-actions>
            </v-card>
        </v-expand-transition> -->
  </v-card>
</template>
<script>
export default {
  data: () => ({
    reveal: false,
  }),
  props: {
    CardData: {
      type: Object,
      required: true,
    },
  },
};
</script>
<style>
.row {
  margin: 0px !important;
}
.v-card--reveal {
  bottom: 0;
  opacity: 1 !important;
  position: absolute;
  width: 100%;
}
#cards {
  color: var(--text-color);
  background-color: var(--primary-color);
}
</style>
