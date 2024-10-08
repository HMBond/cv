<script>
	import MainColumn from './MainColumn.svelte';
	import SideColumn from './SideColumn.svelte';

	export const sideColumn = [
		{
			type: 'contact',
			label: 'Contact',
			details: [
				{
					subcategory: 'details',
					contactDetails: [
						{
							isLink: true,
							type: 'email',
							text: 'hubertusmariabond@gmail.com',
							icon: 'email',
						},
						{
							isLink: true,
							type: 'phone',
							text: '+31654316094',
							icon: 'phone',
						},
					],
				},
				{
					subcategory: 'Social media',
					contactDetails: [
						{
							isLink: true,
							type: 'web',
							url: 'mrsunshine.live',
							text: 'mrsunshine.live',
							icon: 'user',
						},
						{
							isLink: true,
							type: 'web',
							url: 'github.com/hmbond',
							text: 'github.com/hmbond',
							icon: 'github',
						},
						{
							isLink: true,
							type: 'web',
							url: 'www.linkedin.com/in/mike-bond-3258a32a/',
							text: 'linkedin.com/in/hmbond',
							icon: 'linkedin',
						},
					],
				},
			],
		},
		{
			type: 'skills',
			label: 'Skills',
			details: [
				'Typescript',
				'ESNext',
				'React',
				'Next',
				'Svelte',
				'Ruby on Rails',
				'.NET / Blazor',
				'Neo4j',
				'NeonDb',
				'SQL',
				'Node',
				'Bun',
				'C#',
				'HTML',
				'CSS',
				'zsh',
			],
		},
		{
			type: 'simple-details',
			label: 'Projects',
			details: [
				{
					title: 'Towards the Artist',
					url: 'soundcloud.com/towardstheartist',
					link: 'soundcloud.com/towardstheartist',
					icon: 'music',
					description:
						'Recording local artists and presenting their works online.',
				},
				{
					title: 'Unity Exhibition',
					url: 'humanityhouse.org/',
					link: 'humanityhouse.org/',
					icon: 'eye',
					description:
						'Coding and building an interactive art installation to state the importance of privacy and identity.',
				},
				{
					title: 'Volunteering',
					icon: 'heart',
					description:
						'Previous board member of a people society in Delft and two living groups. <a target="_blank" href="https://wolpop.nl">Organizing concerts</a> and volunteering at festivals and the <a target="_blank" href="https://www.designresearchsociety.org/">DRS Conference 2014</a>.',
				},
			],
		},
	];
	export const mainColumn = [
		{
			type: 'full-details',
			label: 'Experience',
			details: [
				{
					title: 'Senior Full-Stack Developer',
					subtitle: 'Thoughtworks',
					dates: `4/2021 - 2/2024`,
					location: 'Berlin, Germany',
					description:
						'Working on an internal application for one of the mayor automotive companies.',
					list: [
						'Advocating to code for <a target="_blank" href="https://www.thoughtworks.com/insights/topic/accessibility">accessibility</a> by organizing practical workshops.',
						'Building new features within a complex business context.',
						'Improving code quality by removing technical depth and implementing guidelines and a common coding style.',
					],
				},
				{
					title: 'Freelancer',
					subtitle: 'The Bond Experience',
					dates: `5/2019 - 3/2022`,
					location: 'Delft, The Netherlands',
					description:
						'Working as freelancer to produce small web apps and immersive background music for theater/social interaction projects.',
					list: [
						'Various music productions for <a target="_blank" href="https://smeltsmelt.nl/">SMELT</a> performances',
						'Working on a <a target="_blank" href="https://mrsunshine.live/mmc">modular midi controller</a>',
					],
				},
				{
					title: 'Senior Front-end Developer',
					subtitle: 'IX Technologies B.V.',
					dates: '2/2020 - 7/2021',
					location: 'Delft, The Netherlands',
					description:
						'Maintaining serious games and admission tests/simulations for clients in research and air traffic control (ATC). Exploring technical possibilities within a tech-stack transition and working in a small team, directly involved with the clients.',
					list: [
						'Creating a brand new ATC admission simulation in .NET Blazor.',
						'Developing a custom .NET Blazor component library to be integrated in simulations, tests and the administration platform',
					],
				},
				{
					title: 'Junior Front-end Developer',
					subtitle: 'Mobiel.nl',
					dates: '8/2018 — 7/2019',
					location: 'Leidschendam, The Netherlands',
					description:
						'Learning the ins and outs of modern front-end development from experts in the field.',
					list: [
						'Daily code-reviews and working in a Scrum Team.',
						'Working with React, MobX and Ruby on Rails.',
					],
				},
			],
		},
		{
			type: 'full-details',
			label: 'Education',
			details: [
				{
					title: 'Msc. Design for Interaction',
					subtitle: 'TU-Delft',
					dates: '2013 - 2016',
					location: 'Delft, The Netherlands',
				},
				{
					title: 'Bsc. Industrial Design',
					subtitle: 'TU-Delft',
					dates: '2006 - 2011',
					location: 'Delft, The Netherlands',
				},
				{
					title: 'Minor Physics Education',
					subtitle: 'TU-Delft',
					dates: '2009',
					location: 'Delft, The Netherlands',
				},
			],
		},
	];
</script>

<div class="main-body">
	<MainColumn sections={mainColumn} />
	<SideColumn sections={sideColumn} />
</div>

<style>
	div {
		display: flex;
		justify-content: space-between;
		flex-direction: var(--column-order);
		margin: 0 var(--horizontal-offset);
	}
</style>
