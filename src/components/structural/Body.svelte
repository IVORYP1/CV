ne<script>
	import SideColumn from './SideColumn.svelte';
	import MainColumn from './MainColumn.svelte';

	export const sideColumn = [
		{
			type: 'contact',
			label: 'Contact',
			details: [
				{
					subcategory: 'Say hi',
					contactDetails: [
						{
							isLink: true,
							type: 'email',
							text: 'ivorypeter77@gmail.com',
							icon: 'email',
						},
						{
							isLink: true,
							type: 'phone',
							text: '(+64)0224562367',
							icon: 'phone',
						},
						{
							text: 'Hawkes Bay, New Zealand',
							icon: 'location',
						},
					],
				},
				{
					subcategory: 'Find me online',
					contactDetails: [
						{
							isLink: true,
							type: 'web',
							url: 'IO-website.com',
							text: 'IO-website.com',
						},
						{
							isLink: true,
							type: 'web',
							url: 'https://github.com/PeterSomething',
							text: 'github.com/PeterSomething',
							icon: 'github',
						},
						{
							isLink: true,
							type: 'web',
							url: 'https://www.linkedin.com/in/peter-ivory-99805518b/',
							text: '.linkedin.com/in/peter-ivory',
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
				'PostgreSQL',
				'MySQL',
				'SQL server',
				'HTML',
				'CSS',
				'Git',
				'Bootstrap',
				'Data analytics',
				'Power BI',
				'orange',
				'python',
				'YOLOv5',
				'Donkey Car application',
				'Bubble',
				'JavaScript',
			    	//'Jira',
				'MongoDB'
			],
		},
		{
			type: 'simple-details',
			label: 'Projects',
			details: [
				{
					title: 'Liv-City',
					url: 'https://2020.hackerspace.govhack.org/projects/livcity',
					link: 'Liv-City.com',
					description:
						'This was a project done for 2020 New Zealand Gov Hack competion, in the form of a mobile application which used flutter as its base in which i came up with the wireframes and database design.',
				},
				{
					title: 'Localé',
					url: 'http://bit.ly/2Ix2sKW',
					link: 'newsmashed.herokuapp.com',
					description:
						'This was a 2019 New Zealnd Gov Hack comptetion in which we creted a front end and backend website for finding events and deciding what events are available in a city, in this project i worked maoinly on the wireframes and video.',
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
					title: 'Partner',
					subtitle: 'ioSoftworks',
					dates: 'Febuary 2021 — Present',
					location: 'Hastings, New Zealand',
					description: 'Software as a service ',
					list: [
						'Worked towards ensuring database integrity.',
						'Worked in a team to analyze data to create new revenue streams.',
						'Built tools to visualize data to increase company reputation.',
					],
				},
				{
					title: 'Intern',
					subtitle: 'Fingermark Full time Intern',
					dates: `November 2020 - Febuary 2021`,
					location: 'Havelock North, New Zealand',
					description: 'Worked on migrating the Database',
					list: [
						'Finding and researching ways to fix errors in the PosgresSQL database.',
						'Testing migration and database analytics tools.',
						'Constructed Fake database instances to test out migrations of data.',
						'Layed the groundwork for a full database migration using PostgreSQL',
						'Labelled data for machine learning using CVAT',

						// 'Implement product rating system to handle both numerical reviews and comments',
						// Use React.js to add prompts and visual cues for shoppers to update product and inventory information.
						// Contracted to develop tech stack focused on MongoDB, Express.js, React, Node.js.
					],
				},
				
				//{
				//	title: 'Math Fellow, Americorps',
				//	subtitle: 'Denver Public Schools',
				//	dates: '2017 — 2018',
				//	location: 'Denver, CO',
			//		description: 'Middle school math intervention program',
				//	list: [
				//		'Improved academic outcomes for a diverse student population by creating and teaching lesson plans that included original worksheets and activities.',
				//		'Developed a positive motivation system to encourage on-task behavior, teamwork, and delaying of rewards.',
			//			'Launched and led HTML coding enrichment class with Galvanize students.',
						// • Taught small-group 6th grade math intervention, writing and delivering original lessons.
						// • Managed behavior and relationships with a positive motivation system, restorative conversations, and supplemental tutoring.
						// • Facilitated an elective with Galvanize where students learned HTML and built websites (deployed and hosted by Galvanize).
			//		],
				//},
			//	{
			//		title: 'Technical Writer',
			//		subtitle: 'KBC Advanced Technologies',
			//		dates: '2014 — 2015',
			//		location: 'Denver, CO',
			//		description: 'Oil refinery operations manuals',
			//		list: [
			//			'Produced high quality training manuals that included written content and Visio drawings, synthesizing information from various sources.',
			//		],
			//	},

				// Linkedin

					// 'Produced high quality training manuals for oil refinery operations to communicate how materials move through complex systems.',
					// 'Wrote clear, concise content with information compiled from client documents, photos, and detailed flow diagrams.'
					// 'Created Visio drawings of condensed stream and equipment information to assist with visual understanding.',

				// Honeybee Robotics, New York, NY
				// Operations Associate, 2012–2013
				// • Controlled project document streams and managed all incoming bills, serving as the main point of contact for vendors.
				// • Created a macro in Excel VBA to automate entry and processing of expense data.
				// • Updated and expanded company website and blog using Joomla!
			],
		},
		{
			type: 'full-details',
			label: 'Education',
			details: [
				{
					title: 'Bachelor of Computer Systems',
					subtitle: 'Eastern Institute of Technology',
					dates: 'End date 2021',
					location: 'Napier New Zealand',
				},
			],
		},
	];
</script>

<style>
	div {
		display: flex;
		justify-content: space-between;
		flex-direction: var(--column-order);
		margin: 0 var(--horizontal-offset);
	}
</style>

<div class="main-body">
	<MainColumn sections={mainColumn} />
	<SideColumn sections={sideColumn} />
</div>
