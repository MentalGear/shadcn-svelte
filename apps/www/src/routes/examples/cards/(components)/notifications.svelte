<script lang="ts">
	import Bell from "svelte-radix/Bell.svelte";
	import EyeNone from "svelte-radix/EyeNone.svelte";
	import Person from "svelte-radix/Person.svelte";
	import * as Card from "@/registry/new-york/ui/card";
</script>

<Card.Root>
	<Card.Header class="pb-3">
		<Card.Title>Notifications</Card.Title>
		<Card.Description>Choose what you want to be notified about.</Card.Description>
	</Card.Header>
	<Card.Content class="grid gap-1">
		<div
			class="-mx-2 flex items-start space-x-4 rounded-md p-2 transition-all hover:bg-accent hover:text-accent-foreground"
		>
			<Bell class="mt-px h-5 w-5" />
			<div class="space-y-1">
				<p class="text-sm font-medium leading-none">Everything</p>
				<p class="text-sm text-muted-foreground">Email digest, mentions & all activity.</p>
			</div>
		</div>
		<div
			class="-mx-2 flex items-start space-x-4 rounded-md bg-accent p-2 text-accent-foreground transition-all"
		>
			<Person class="mt-px h-5 w-5" />
			<div class="space-y-1">
				<p class="text-sm font-medium leading-none">Available</p>
				<p class="text-sm text-muted-foreground">Only mentions and comments.</p>
			</div>
		</div>
		<div
			class="-mx-2 flex items-start space-x-4 rounded-md p-2 transition-all hover:bg-accent hover:text-accent-foreground"
		>
			<EyeNone class="mt-px h-5 w-5" />
			<div class="space-y-1">
				<p class="text-sm font-medium leading-none">Ignoring</p>
				<p class="text-sm text-muted-foreground">Turn off all notifications.</p>
			</div>
		</div>
	</Card.Content>
</Card.Root>
