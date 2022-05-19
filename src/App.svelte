<script>
	import Page from "./Page.svelte";

	let info = {
		name: "Saner | Kinoshi",
		description: "I'm a web developer",
		socialmedia: [
			{
				key: "İnstagram",
				value: "https://www.instagram.com/kinoshisocial/"
			},
			{
				key: "Github",
				value: "https://github.com/kinoshisocial"
			},
			{
				key: "Discord",
				value: "https://discord.com/users/913076582694944839"
			}
		]
	}

</script>

<Page user={info} />
