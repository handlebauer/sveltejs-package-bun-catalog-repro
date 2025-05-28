<script>
  export let variant = 'primary';
  export let disabled = false;
</script>

<button class="btn btn-{variant}" {disabled} on:click>
  <slot />
</button>

<style>
  .btn {
    padding: 0.5rem 1rem;
    border: none;
    border-radius: 0.25rem;
    cursor: pointer;
    font-weight: 500;
  }
  
  .btn-primary {
    background-color: #3b82f6;
    color: white;
  }
  
  .btn-secondary {
    background-color: #6b7280;
    color: white;
  }
  
  .btn:disabled {
    opacity: 0.5;
    cursor: not-allowed;
  }
</style> 