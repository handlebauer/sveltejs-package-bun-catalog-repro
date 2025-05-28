<script>
  export let title = '';
  export let subtitle = '';
</script>

<div class="card">
  {#if title}
    <h3 class="card-title">{title}</h3>
  {/if}
  {#if subtitle}
    <p class="card-subtitle">{subtitle}</p>
  {/if}
  <div class="card-content">
    <slot />
  </div>
</div>

<style>
  .card {
    border: 1px solid #e5e7eb;
    border-radius: 0.5rem;
    padding: 1rem;
    background-color: white;
    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
  }
  
  .card-title {
    margin: 0 0 0.5rem 0;
    font-size: 1.25rem;
    font-weight: 600;
  }
  
  .card-subtitle {
    margin: 0 0 1rem 0;
    color: #6b7280;
    font-size: 0.875rem;
  }
  
  .card-content {
    margin: 0;
  }
</style> 