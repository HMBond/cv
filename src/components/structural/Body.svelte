<script>
	import MainColumn from './MainColumn.svelte';

	export const mainColumn = [
		{
			type: 'full-details',
			label: 'Mike Bond',
			details: [
				{
					description: `Meester Muhrenlaan 68\n1132CH, Volendam\n<a href="mailto:hubertusmariabond@gmail.com" target="_blank">hubertusmariabond@gmail.com</a>\n<a href="tel:0654356094">0654356094</a>`,
				},
				{
					description: 'Beste HR-medewerker,',
				},
				{
					description:
						'Ik heb interesse het werken als Front End Developer bij de ANWB. Met ruim 5 jaar werkervaring als developer en een Msc. in Interaction Design, sluiten mijn professionele vaardigheden goed aan bij de vacature. Aangezien de ANWB een breed scala aan producten aanbiedt en de complexiteit van <a href="https://www.anwb.nl/" target="_blank">ANWB.nl</a> groot is, lijkt het erop dat er zeer kundig gewerkt wordt binnen de development-afdeling.',
				},
				{
					description:
						'Daarnaast vind ik de ANWB een bedrijf met een mooie uitstraling, en ben ik zelf recent lid geworden van de Wegenwacht-service. Ooit heb ik nog de typische gele rugzak van de ANWB gedragen als student! Ik beschouw de ANWB als een eerlijk bedrijf met kwaliteitsproducten.',
				},
				{
					description: `Als Front End Developer draag ik bij aan een nette, duidelijke en fijne werksfeer, zowel in het afleveren van code als in de omgang met collega’s`,
				},
				{
					description: `Het is voor mij belangrijk om mezelf op de hoogte te houden van de laatste ontwikkelingen in webtechnologieën (via <a href="https://www.thoughtworks.com/radar" target="_blank">Technology Radar</a>, <a href="https://daily.dev/" target="_blank">Daily.dev</a> en nieuwsbrieven) zodat ik actief kan bijdragen aan vernieuwing en onderhoud van technologie. Ik breng graag complexe (business)processen in kaart om vervolgens samen met het team op basis van genuanceerde beslissingen problemen op te lossen. Om dit zowel nu als in de toekomst zo soepel mogelijk te laten verlopen, pleit ik voor een Clean Code mentaliteit, Agile werkmethoden en een optimale CI/CD-architectuur.`,
				},
				{
					description: `In de omgang ben ik een zeer sociaal persoon om samen mee te werken. Ik waardeer eerlijke feedback en evaluaties in een vrolijke sfeer waar ook gelachen kan worden. Aan een vrolijke sfeer draag ik graag aan bij met het geven van boventonenzang workshops, (tech) demo's, fotografie en hulp bij festiviteiten. In mijn vrije tijd ontwikkel ik een app voor interactieve muziek en speel verschillende instrumenten.`,
				},
				{
					description: `Ik zou het heel fijn vinden om bij te dragen aan de digitale services van de ANWB en geloof dat ik jullie blij kan maken met mijn enthausiastme, kennis en expertise in webdevelopment.`,
				},
				{
					description:
						'Dankjewel voor de interesse in mijn reactie op de vacature en vriendelijke groet,\n\nMike Bond',
				},
			],
		},
	];
</script>

<div class="main-body">
	<MainColumn sections={mainColumn} />
</div>

<style>
	div {
		display: flex;
		justify-content: space-between;
		flex-direction: var(--column-order);
		margin: 0 var(--horizontal-offset);
	}
</style>
