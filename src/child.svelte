<script>
    import { getNotificationsContext } from 'svelte-notifications';
    const { addNotification } = getNotificationsContext();
    export let selectedTheme;
</script>

<button class="notification {selectedTheme}"
  on:click={() => addNotification({
    text: 'This is a test notification',
    position: 'top-right',
  })}
	>
	Notification Experiment
</button>

<style>
  button {
    border-radius: 5pt;
    color: black;
  }
</style>