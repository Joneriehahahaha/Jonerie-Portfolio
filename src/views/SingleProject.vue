<script>
import feather from 'feather-icons';
import ProjectHeader from '../components/projects/ProjectHeader.vue';
import ProjectGallery from '../components/projects/ProjectGallery.vue';
import ProjectInfo from '../components/projects/ProjectInfo.vue';
import ProjectRelatedProjects from '../components/projects/ProjectRelatedProjects.vue';

export default {
	name: 'Projects',
	components: {
		ProjectHeader,
		ProjectGallery,
		ProjectInfo,
		ProjectRelatedProjects,
	},
	data: () => {
		return {
			singleProjectHeader: {
				singleProjectTitle: 'Pixel Management UI',
				singleProjectDate: 'Apr 7, 2024',
				singleProjectTag: 'UI / Frontend',
			},
			projectImages: [
				{
					id: 1,
					title: '',
					img: require('@/assets/images/xx.jpg'),
				},
				{
					id: 2,
					title: 'Pixel',
					img: require('@/assets/images/paldo.jpg'),
				},
				
			],
			projectInfo: {
				clientHeading: 'About Pixel',
				companyInfos: [
					{
						id: 1,
						title: 'Name',
						details: 'PixelGaming.xyz',
					},
					{
						id: 2,
						title: 'Services',
						details: 'UI Design & Frontend Development',
					},
					{
						id: 3,
						title: 'Website',
						details: 'https://pixelgaming.xyz',
					},
					{
						id: 4,
						title: 'Phone',
						details: '666 999 666',
					},
				],
				objectivesHeading: 'Objective',
				objectivesDetails:
					'Play pixel to earn money',
				technologies: [
					{
						title: 'Tools & Technologies',
						techs: [
							'HTML',
							'CSS',
							'JavaScript',
							'Vue.js',
							'TailwindCSS',
							'AdobeXD',
						],
					},
				],
				projectDetailsHeading: 'An Infinite World of Endless',
				projectDetails: [
					{
						id: 1,
						details:
							'Pixel gaming has experienced a resurgence in popularity in recent years, partly due to nostalgia for retro gaming aesthetics and partly due to the accessibility of pixel art creation tools for indie developers. Many indie games, as well as some mainstream titles, employ pixel art to evoke a sense of nostalgia or to create unique visual styles.',
					},
					{
						id: 12,
						details:
							'Pixel gaming isn`t limited to a specific genre; it can encompass a wide range of game types, including platformers, RPGs, action-adventure games, puzzle games, and more. Some well-known examples of pixel art games include "Minecraft," "Stardew Valley," "Undertale," "Celeste," and "Hyper Light Drifter," among many others.'
					},
						
				],
				socialSharingsHeading: 'Share This',
				socialSharings: [
					{
						id: 1,
						name: 'Twitter',
						icon: 'twitter',
						url: 'https://twitter.com/JonerieJr',
					},
					{
						id: 2,
						name: 'Instagram',
						icon: 'instagram',
						url: 'https://www.instagram.com/jn.rein/',
					},
					{
						id: 3,
						name: 'Facebook',
						icon: 'facebook',
						url: 'https://www.facebook.com/j.020720',
					},
					
				],
			},
			relatedProject: {
				relatedProjectsHeading: '',
				relatedProjects: [
					
					
				],
			},
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div class="container mx-auto mt-10 sm:mt-20">
		<!-- Project header -->
		<ProjectHeader :singleProjectHeader="singleProjectHeader" />

		<!-- Project gallery -->
		<ProjectGallery :projectImages="projectImages" />

		<!-- Project information -->
		<ProjectInfo :projectInfo="projectInfo" />

		<!-- Project related projects -->
		<ProjectRelatedProjects :relatedProject="relatedProject" />
	</div>
</template>

<style scoped></style>
