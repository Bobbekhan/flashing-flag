<style>
@keyframes flash {
  0% { opacity: 1; }
  50% { opacity: 0.5; }
  100% { opacity: 1; }
}

body {
  margin: 0;
  padding: 0;
  background-color: #000;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.flag {
  animation: flash 1s infinite;
  max-width: 100%;
  max-height: 100%;
  object-fit: contain;
}
</style>
