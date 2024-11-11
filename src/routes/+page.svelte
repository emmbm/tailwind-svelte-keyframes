<p class="without-prefix">This should animate using global keyframes defined within the component using the prescribed <code>-global-</code> prefix.</p>
<p class="with-prefix">This should <b>not</b> animate as the keyframes' name should be stripped of the <code>-global-</code> prefix.</p>

<style>
  @keyframes -global-test {
    0%,100% {
      opacity: 0;
    }
    50% {
      opacity: 100%;
    }
  }

  .without-prefix {
    animation: 2s ease-in-out 0s infinite test;
  }

  .with-prefix {
    animation: 2s ease-in-out 0s infinite -global-test;
  }
</style>
