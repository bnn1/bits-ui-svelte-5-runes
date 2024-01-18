<script lang="ts">
	import { Avatar as AvatarPrimitive } from 'bits-ui';
	import { cn } from '@lib/utils';

	const { src, alt, class: className, ...rest } = $props<AvatarPrimitive.ImageProps>();
</script>

<AvatarPrimitive.Image {src} {alt} class={cn('aspect-square h-full w-full', className)} {...rest} />
