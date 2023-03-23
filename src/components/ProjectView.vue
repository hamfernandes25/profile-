<template>
  <div>
    <v-container fluid>
      <v-card>
        <v-img
          class="align-end text-white"
          height="200"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
          cover
        >
          <v-card-title>Projects</v-card-title>
        </v-img>

        <v-card-text class="pt-1">
          Sluice Gates – Automated Water Flow Control System(IoT based)” which
          won best project of year of IT department
        </v-card-text>

        <v-card-text>
          <div>
            Automated Sluice Gate involves mechanically powered opening and
            closing the sluice gates using Raspberry-Pi microcontrollers and
            servo motors. It will also do away with the hassles of manually
            going to the site and operating it and the use of IoT ensures time
            saving and Man power reduction. It is an excellent water level
            control mechanism and is more efficient
          </div>
          <div>
            Modules : Web Application module for communication between the
            android application and the raspberry-pi and to collect and store
            data collected from sensors for analysis purpose and to notify the
            user through GCM notifications. On site module containing ultrasound
            sensors, raspberry-pi , servo motors and sluice gates. Android
            application for controlling which gates to open/close
          </div>
          <div>Technologies used – Android, Python, PHP, MySQL, Google GCM</div>
          <div>
            Roles and Responsibilities – Developer, Team Lead, managing team
            activities, reporting to project guide/mentor and project
            documentation
          </div>
        </v-card-text>
      </v-card>
    </v-container>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import CardView from './card.vue'

export default {
  name: "ProjectView",
  components: {
    // HelloWorld,
    // CardView,
  },
};
</script>
