<template>
  <div class="cal-modal-wrap" @click.self="$emit('done')">
    <div class="cal-modal">
      <div class="close-btn" @click="$emit('done')">close</div>
      <iframe
        src="https://calendar.google.com/calendar/embed?height=800&amp;wkst=1&amp;bgcolor=%23ffffff&amp;ctz=America%2FChicago&amp;src=ZWFtYXR6MjRAZ21haWwuY29t&amp;src=aThzOGYydXJkMW03YmFzZXBzZnZtdjZ1MTBAZ3JvdXAuY2FsZW5kYXIuZ29vZ2xlLmNvbQ&amp;color=%23F09300&amp;color=%232d97cc&amp;mode=WEEK&amp;showCalendars=0&amp;showPrint=0&amp;showDate=1&amp;showNav=1"
        class="cal-iframe"
        style="border-width:0"
        width="1024"
        height="800"
        frameborder="0"
        scrolling="no"
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.cal-modal-wrap {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgba(128, 128, 128, 0.75);
}
.cal-modal {
  background-color: white;
  padding: 50px;
  position: relative;
  border-radius: 16px;
}
.cal-iframe {
  max-width: calc(90vw - 100px);
  max-height: calc(90vh - 100px);
}
.close-btn {
  position: absolute;
  top: 12px;
  right: 24px;
  cursor: pointer;
  color: blue;
}
</style>