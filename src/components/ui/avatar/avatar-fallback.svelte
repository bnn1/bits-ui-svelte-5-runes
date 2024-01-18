<script lang="ts">
	import { Avatar as AvatarPrimitive } from 'bits-ui';
	import { cn } from '@lib/utils';

	const { class: className, ...rest } = $props<AvatarPrimitive.FallbackProps>();
</script>

<AvatarPrimitive.Fallback
	class={cn('flex h-full w-full items-center justify-center rounded-full bg-muted', className)}
	{...rest}
>
	<slot />
</AvatarPrimitive.Fallback>
