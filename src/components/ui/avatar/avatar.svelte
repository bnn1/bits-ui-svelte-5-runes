<script lang="ts">
	import { Avatar as AvatarPrimitive } from 'bits-ui';
	import { cn } from '@lib/utils';

	const { class: className, delayMs, ...rest } = $props<AvatarPrimitive.Props>();
</script>

<AvatarPrimitive.Root
	{delayMs}
	class={cn('relative flex h-10 w-10 shrink-0 overflow-hidden rounded-full', className)}
	{...rest}
>
	<slot />
</AvatarPrimitive.Root>
