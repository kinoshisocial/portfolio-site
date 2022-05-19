<script>
	import Page from "./Page.svelte";

	let info = {
		name: "Saner | Kinoshi",
		description: "I'm a web developer",
		socialmedia: {
			instagram: "https://www.instagram.com/kinoshisocial/",
			github: "https://github.com/kinoshisocial",
			discord: "https://discord.com/users/913076582694944839"
		}
	}

</script>

<Page user={info} />