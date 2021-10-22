<script>
    import { getNotificationsContext } from 'svelte-notifications';
    const { addNotification } = getNotificationsContext();
</script>

<button
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
  }
</style>