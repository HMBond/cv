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
							url: 'bondux.mrsunshine.live',
							text: 'bondux.dev',
							icon: 'user',
						},
						{
							isLink: true,
							type: 'web',
							url: 'mrsunshine.live',
							text: 'mrsunshine.live',
							icon: 'music',
						},
						{
							isLink: true,
							type: 'web',
							url: 'github.com/hmbond',
							text: 'GitHub profile',
							icon: 'github',
						},
						{
							isLink: true,
							type: 'web',
							url: 'www.linkedin.com/in/mike-bond-3258a32a/',
							text: 'LinkedIn',
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
				'React / Next',
				'Svelte',
				'Angular',
				'Storybook',
				'Stencil',
				'Responsive Web Design',
				'Ruby on Rails',
				'.NET / Blazor',
				'TestCafe',
				'Cypress',
				'Playwright',
				'Jest',
				'Vitest',
				'Neo4j',
				'NeonDb',
				'PostgreSQL',
				'GraphQL',
				'Terraform',
				'Docker',
				'Kubernetes',
				'zsh scripting',
				'Dependency Management',
				'Performance Testing',
				'Node',
				'Bun',
				'C#',
				'Kotlin',
				'HTML',
				'CSS/SASS',
				'PWA',
				'Arduino',
				'Electronics',
				'Scrum / Kanban',
				'Test-Driven Development',
				'Dutch',
				'English',
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
						'Improving architecture and building internal applications for one of the major German automotive companies.',
					list: [
						'Advocate for <a target="_blank" href="https://www.thoughtworks.com/insights/topic/accessibility">accessibility</a> by organizing practical workshops for over 50 developers within the account.',
						'Building new features within a complex business context. Translating client needs into features.',
						'Improving time to production by minimizing technical debt in testing and deployment.',
						'Organizing cross-team sessions to improve code quality.',
					],
				},
				{
					title: 'Freelancer',
					subtitle: 'The Bond Experience',
					dates: `5/2019 - 3/2022`,
					location: 'Delft, The Netherlands',
					description:
						'Working as a freelancer to produce small web apps and immersive background music for theatrical performances and social interaction projects.',
					list: [
						'Various music productions for <a target="_blank" href="https://smeltsmelt.nl/">SMELT</a> performances.',
						'Working on a <a target="_blank" href="https://mmc.mrsunshine.live">modular midi controller</a>.',
					],
				},
				{
					title: 'Senior Front-end Developer',
					subtitle: 'IX Technologies B.V.',
					dates: '2/2020 - 7/2021',
					location: 'Delft, The Netherlands',
					description:
						'Maintaining Air Traffic Control (ATC) admission tests and simulations for Eurocontrol and serious games for research at TNO Delft. Exploring technical possibilities within a tech-stack transition and working in a small team, directly involved with the clients and UX design.',
					list: [
						'Designing and developing the m.v.p. of the renewed ATC simulation in .NET Blazor. This simulation test is now used for all applicants who apply to the ATC training in Europe, Canada, Singapore and other countries.',
						'Developing a custom .NET Blazor component library to be integrated in simulations, tests and the administration platform.',
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
						'Rewriting the product page to use React + MobX and upgrading features together in a small scrum team.',
						'Daily code-reviews and pair programming for a steep learning curve.',
						'Version control, test driven development and deployment in Jenkins.',
						'Fixing backend bugs in Ruby on Rails.',
					],
				},
			],
		},
		{
			type: 'simple-details',
			label: 'Projects',
			details: [
				{
					title: 'MMC-3000',
					url: 'mmc.mrsunshine.live',
					link: 'mmc.mrsunshine.live',
					icon: 'gamepad',
					description:
						'Developing a whiteboard app for creating and sharing MIDI controllers. This enables artists to let the audience control the music.',
				},
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
