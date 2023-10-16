<script setup lang="ts">
import {} from "vue"

import { UserIcon, CpuChipIcon } from "@heroicons/vue/24/solid"

import Top from "./Top.vue"
import Bottom from "./Bottom.vue"
</script>

<template>
	<div class="">
		<Top />
		<div
			class="h-[calc(100vh-8rem)] p-4 border border-red-500 overflow-auto"
		>
			<div class="chat chat-start" v-for="i in 3">
				<div class="chat-image">
					<div
						class="grid place-items-center w-10 aspect-square bg-secondary rounded-full"
					>
						<CpuChipIcon class="w-6 fill-white" />
					</div>
				</div>
				<div class="chat-bubble">
					It was said that you would, destroy the Sith, not join them.
					Lorem ipsum dolor sit amet consectetur, adipisicing elit.
					Reprehenderit ipsum autem labore vitae voluptatibus quae
					voluptatum ducimus consequuntur repudiandae dolores alias,
					ab nihil reiciendis nam accusamus sed dicta suscipit.
					Dolore.
				</div>
			</div>
			<div class="chat chat-end">
				<div class="chat-image">
					<div
						class="grid place-items-center w-10 aspect-square bg-primary rounded-full"
					>
						<UserIcon class="block w-6 fill-white" />
					</div>
				</div>
				<div class="chat-bubble">Not leave it in Darkness</div>
			</div>
		</div>
		<Bottom />
	</div>
</template>
