<script>
  import { url, goto } from "@sveltech/routify";
</script>

<h3>Verify Account</h3>
<p>Please provide the OTP code sent to +630000000 to verify your account.</p>

<div class="form-group">
  <label for="">Mobile Number</label>
  <div class="input-group">
    <div class="input-group-prepend">
      <span class="input-group-text">+63</span>
    </div>
    <input type="text" class="form-control" />
  </div>
</div>

<div class="pt-2">
  <button
    class="btn btn-block btn-primary"
    on:click={() => {
      $goto('/user');
    }}>
    Submit
  </button>
</div>

<div class="pt-3 d-flex">
  <div class="text-left">
    <a href={$url('/')}>Back to login</a>
  </div>
  <div class="flex-grow-1" />
</div>
