<script>
	const value = await Promise.reject(new Error('boom'));
</script>

<h1>{value}</h1>
