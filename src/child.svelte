<script>
    import { getNotificationsContext } from 'svelte-notifications';
    const { addNotification } = getNotificationsContext();
    export let selectedTheme;
</script>

<button class="button:disabled"
  on:click={() => addNotification({
    text: 'This is a test notification',
    position: 'top-right',
  })}
	>
	Experiment #ff01 temporarily disabled
</button>

<style>
  button {
    border-radius: 5pt;
    color: black;
  }
</style>