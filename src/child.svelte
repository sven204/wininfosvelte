<script>
    import { getNotificationsContext } from 'svelte-notifications';
    const { addNotification } = getNotificationsContext();
</script>

<button
  on:click={() => addNotification({
    text: 'Notification',
    position: 'bottom-center',
  })}
	>
	Click me
</button>

<style>
  button {
    border-radius: 5pt;
  }
</style>