<script>
	export let detail;
	let { isLink, type, text, url, icon } = detail;
	let defaultIcon = 'fa fa-star';
	const fontAwesomeIconMap = {
		location: 'fa fa-map-marker',
		email: 'fa fa-envelope',
		phone: 'fa fa-phone-alt',
		github: 'fab fa-github',
		linkedin: 'fab fa-linkedin-in',
		user: 'fa fa-user',
		music: 'fa fa-music',
		gamepad: 'fa fa-gamepad',
		heart: 'fa fa-heart',
		eye: 'fa fa-eye',
	};
	let linkIcon = fontAwesomeIconMap[icon] || defaultIcon;
</script>

<div class="contact-item">
	<i class={linkIcon} />
	{#if isLink}
		{#if type === 'email'}
			<a target="_blank" href="mailto:{text}">{text}</a>
		{:else if type === 'phone'}
			<a target="_blank" href="tel:{text}">{text}</a>
		{:else if url}
			<a target="_blank" href="http://{url}">{text}</a>
		{:else}
			<a target="_blank" href="http://{text}">{text}</a>
		{/if}
	{:else}{text}{/if}
</div>

<style>
	.contact-item i {
		width: 20px;
		padding-right: 5px;
		font-size: 0.9rem;
		text-align: center;
	}

	.contact-item a {
		font-size: 0.9em;
	}

	.full-detail .contact-item i {
		padding-right: 2px; /*	less padding for experience map marker */
	}

	.simple-detail .contact-item {
		margin-top: 5px;
	}
</style>
