<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						"I'm a passionate computer enthusiast and student. I love exploring the vast world of technology, coding, and everything related to computers. From programming to hardware, I find joy in understanding how things work in the digital realm. I'm always eager to learn and stay updated with the latest trends in the tech industry.",
				},
				// {
				// 	id: 2,
				// 	bio:
				// 		'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Nihil vel illum asperiores dignissimos cumque quibusdam et fugiat voluptatem nobis suscipit explicabo, eaque consequatur nesciunt, fugit eligendi corporis laudantium adipisci soluta?',
				// },
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpeg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
