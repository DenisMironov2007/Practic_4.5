<nav>
	<div class="nav-container">
		<a href="/" class="nav-logo">Main</a>
		<div class="nav-links">
			{#each nav as link}
			{#if link.isShow}
				<a href={link.href} class="link">{link.title}</a>
			{/if}
			{/each}
		</div>
	</div>
</nav>
<div class="container">
	<!--Pages will be injected below-->
	<slot></slot>
</div>

<script>
	const nav = [
		{ 
			title: 'About me',
			href: '/about',
			isShow: true
		},
		{
			title: 'Projects',
			href: '/blog',
			isShow: true
		},
		{
			title: 'Task Calendar',
			href: '/task',
			isShow: true
		},
		{
			title: 'Feedback',
			href: '/feedback',
			isShow: true
		},
		{
			title: 'Settings',
			href: '/temp',
			isShow: true
		},
		{
			title: 'Problems_404',
			href: '/ohibka',
			isShow: false
		}
	]
</script>

<style>
	.container {
		max-width: 1400px;
		margin: 50px auto;
	}
</style>