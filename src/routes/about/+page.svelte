<script>
	import Gary from '$lib/assets/gary.jpg';
	import Tony from '$lib/assets/tony.jpg';
	import Justin from '$lib/assets/justin.jpg';
	import Julee from '$lib/assets/julee.jpg';
	import Jungle from '$lib/assets/jungle.jpg';
	import Richrich from '$lib/assets/richrichrich.jpg';

	let items = [
		{
			name: 'Billing Tree',
			text: 'The proven leader in on-demand payment processing, BillingTree simplifies the billing and receivables process. By delivering the most innovative technology and making it as easy and inexpensive as possible to accept payments, BillingTree is revolutionizing the payments landscape. www.mybillingtree.com or call 877.4.BILLTREE.'
		},

		{
			name: 'Client Access Web',
			text: 'Applied Innovations Inc. offers Online Data Access & Payment solutions via web based portals that range from virtual collections & payment processing, to remote client access with state-of-the-art reporting tools, new account entry, & account inquiry tools. Ensure compliance while keeping clients happy and reducing your cost to collect. Website: www.appliedinnovationinc.com/clientaccessweb/'
		},
		{
			name: 'eBureau',
			text: 'Supported by a robust data mining platform that aggregates massive amounts of consumer data, eBureau provides a powerful suite of predictive analytics and real-time information solutions to help agencies, debt buyers and law firms prioritize which accounts to work based on the ability to contact the debtor and the propensity to repay the debt. Website: www.ebureau.com'
		},

		{
			name: 'EFT Network',
			text: "Since 1998, EFT Network has been a leading provider of Electronic Payment Processing solutions for the Collection industry. These innovative payment solutions help agencies reduce operating expenses while automating payment processing and posting, for faster more efficient – and profitable - collections. Today, EFT Network has over 2,000 agencies processing payments electronically. These unparalleled payment processing solutions – along with EFT Network's technical expertise - ensure customized, flawless integration with Debt$Net. Website: www.eftnetwork.com"
		},
		{
			name: 'Focus1 ',
			text: 'Focus1 is a full service commercial print company that offers specialized collection letters and data hygiene services to the debt collection industry. We have derived a system that provides the highest quality data cleanse prior to printing and mailing your custom layout collection letters. Website: www.focus1data.com'
		},

		{
			name: 'SmartDial® technology solutions',
			text: '	From predictive dialers to smart automatic dialers and broadcast messaging, IAT offers a comprehensive variety of SmartDial® technology solutions designed specifically for the collections industry. Our collections experts can tailor a solution for your operations using powerful site-premised predictive dialing systems, hosted dialer services, or a combination of both. Website: www.IATSmartDial.com'
		},
		{
			name: 'LexisNexis ',
			text: 'LexisNexis Receivables Management Solutions delivers a powerful suite of tools that help collections organizations increase right-party contact, improve operational efficiency, minimize risk, and maximize recovery. With over 30 years of experience in data management, LexisNexis has the relevant, current debtor information and the broadest and deepest debtor insight in the industry. 1.866.528.0780 or visit risk.lexisnexis.com/collections.'
		},
		{
			name: 'Payscout ',
			text: '	Payscout specializes in providing Credit Card & Check Processing Accounts to, and dramatically reducing fees and costs for, the Collections Industry. Payscout offers all types of processing accounts, including Credit /Debit Cards, ACH/Check by Phone, Web Payments, Remote Deposit, IVR, and much more, and has done so for some of the best known agencies in the country for many years. Payscout processing solutions have functionalities and options that are unique to Payscout, and that are specifically designed for Collection Agencies. Payscout does not take a “one size fits all” approach in providing accounts, whether you are a small start-up agency, or one that is large and well established, Payscout has the programs that best fit your individual needs. www.payscout.com/debt-collection-credit-card-processing or call 888-689-6088.'
		},
		{
			name: 'Paystream ',
			text: '	Applied Innovations Inc. offers Online Data Access & Payment solutions via web based portals that range from virtual collections & payment processing, to remote client access with state-of-the-art reporting tools, new account entry, & account inquiry tools. Ensure compliance while keeping clients happy and reducing your cost to collect. Website: www.appliedinnovationinc.com/paystream/'
		},

		{
			name: 'RevSpring',
			text: '	RevSpring was formed by the merger of DANTOM Systems, PSC Info Group, Data Image and BestBill. Its core service offerings include data hygiene and analytics, secure document creation and delivery, multi-channel communications, electronic billing and archival services and online payment tools, all while ensuring compliance with regulatory guidelines. Website: www.revspringinc.com'
		},
		{
			name: 'SunGard',
			text: '	SunGard’s AvantGard Predictive Metrics can help increase profits by enhancing debt recovery success and strategically target accounts for legal. Debt collectors can use statistical scoring models to help prioritize collection efforts and improve collection strategies. www.sungard.com'
		},
		{
			name: 'TCN',
			text: "Today, agencies need to do more with less-By using TCN's Cloud-based Predictive Dialing tools and services, agencies can leverage the most sophisticated Outbound and Inbound calling technologies available, leveraging the cloud, all without capital outlay or new staff. Using TCN's revolutionary technologies, agencies can dramatically improve results and ROI. www.tcnp3.com"
		},
		{
			name: 'TriVium ',
			text: "Established in 1996, TriVium Systems is a leading provider of call recording and reporting applications for the account receivables marketplace. We serve hundreds of collection agencies and law firm customers and are affiliated with the industry's leading associations including ACA, NARCA and DBA. www.collections-callrecording.com"
		},

		{
			name: 'UMS Banking/ACH Solutions',
			text: 'UMS Banking/ACH Solutions provides the perfect combination of payment options for the collection industry. Our solutions include credit cards and ACH payments in a variety of forms from web-based, to Virtual Terminal, to Phone Payments, to Face-to-Face - all at the lowest interchange possible. We work with you to make payments easy. From one-time payments to a scheduled payment plan for your clients, to e-invoicing and more, we offer the widest range of payment options in the industry. Additionally, we specialize in B2B software and reduced B2B pricing. All backed by 30 years of experience in the payments industry. www.umsbanking.com'
		},
		{
			name: 'VoApps ',
			text: 'VoApps is the creator of DirectDrop Voicemail Service which delivers a voice message directly to the consumers voicemail box without making a voice call to the mobile handset. The patented DirectDrop Voicemail Service has changed the economics of call centers. Our clients have realized an increase of dollars collected, higher liquidation rates, and more inbound phone calls. Over 100 million messages have been delivered to mobile users with DirectDrop Voicemail and that number grows daily! www.VoApps.com or call 855-737-1596'
		}
	];
	let selected = 'Billing Tree';
	let select = (name) => (selected = name);
</script>

<h1>About</h1>

<img_Intro>
	<img src={Jungle} alt="background" />

	<div class="text_Block">
		<p class="text_Box">
			Founded in 1987 by principals Tony LaMagna and Gary Grout, the company has developed and
			provides the industry their premier core product, Debt$Net®, as well as supporting software
			modules, training, custom programming and technical support.
		</p>

		<p class="text_Box glass_Back">
			Debt$Net®, created by The Computer Manager, Inc., has provided collection agencies, law
			firms, debt buyers and in-house collection departments with one of the most comprehensive debt
			collection systems in the industry. Proven in the field, Debt$Net® collection software has
			satisfied the debt recovery requirements for over 1,000 companies specializing in Retail,
			Commercial, Medical, Receivables Management and Check Collections. Debt$Net® users can be
			found throughout the United States and Canada.
		</p>
	</div>
</img_Intro>

<h2>Sales Approach</h2>
<div class="text_Block">
	<img class="backBack" src={Richrich} alt="background" />
	<p class="text_Box overLay glass_Back">
		Our interactive sales approach ensures a tailored fit between your company and Debt$Net®
		software. Start with our videos for a basic fit assessment. If interested, contact our marketing
		staff for more information and to begin a comprehensive software analysis. Work closely with our
		trainers, well-versed in collection industry needs, during the analysis. Guided Walk-Thrus
		showcase how Debt$Net® meets your business practices and handles various procedures. Categories
		include agency configuration, client screens, debtor and account screens, collection management,
		trust accounting, administrative procedures, and IT staff support. After evaluation, our
		marketing staff provides a customized price quote package for your company's needs. At The
		Computer Manager, Inc., we value your confidence in Debt$Net® collection software.
	</p>

	<h2>Workforce</h2>
	<workforce>
		<div class="img_Face">
			<img src={Gary} alt="background" />
		</div>

		<p class="text_Box glass_Back">
			Gary Grout, Principal, Vice President, and Senior Systems Analyst's business and computer
			science experience encompass more than 30 years of programming, analysis, and supervising. As
			the Principal, Vice President, and Senior Systems Analyst for The Computer Manager, Inc., he
			continually strives to provide their clients with software products that improve their
			productivity and profitability. Gary's technical writing includes the book Business Computing
			for Small Contractors (Osborne/McGraw-Hill, Berkeley, CA, 1986), and numerous articles and
			reviews for such publications as PC Magazine and Creative Computing Magazine.The Computer
			Sciences Corporation named him Employee of the Year for 1989 for his region.
		</p>

		<div class="img_Face">
			<img src={Tony} alt="background" />
		</div>

		<p class="text_Box">
			Anthony C. La Magna, Principal and Corporate Manager, has business experience including more
			than 30 years of operating and managing businesses in the computer and construction
			industries. Tony has had significant impact on profitability and growth as the managing
			principal at The Computer Manager, growing the company from six employees to a top national
			marketer of PC-based collection agency software. Mr. La Magna's computer experience includes
			18 years as a principal of companies formed to provide accounting services to small business
			and to provide consulting and programming services to both government and business clients. As
			President and member of the Board of Directors of the local chapter of the Washington Home
			Builders Association, Tony was voted Builder of the Year in 1984.
		</p>

		<div class="img_Face">
			<img src={Julee} alt="background" />
		</div>

		<p class="text_Box glass_Back">
			Julee Warner, Operations Manager, has been with The Computer Manager, Inc. for over 21 years.
			Her experience with small group dynamic facilitation, business management, human resources,
			curriculum development, and incorporating development strategies helps ensure successful
			operations. She holds a Bachelor's degree in Multidisciplinary Studies from Eastern Oregon
			University.
		</p>

		<div class="img_Face">
			<img src={Justin} alt="background" />
		</div>

		<p class="text_Box">
			Justin Brien, Technical Support Manager, has over 18 years experience resolving Debt$Net®
			clients' technical issues and training new Debt$Net® users. He has extensive knowledge in
			daily processes of a collection agency and collection department. Justin has a Bachelor's
			degree in Business Administration – Management Information Systems from Western Washington
			University.
		</p>
	</workforce>
</div>

<h2>Affiliates</h2>

<ul class="affiliates">
	{#each items as item (item.name)}
		<li
			class={selected === item.name ? 'selected' : 'unselected'}
			on:click={() => select(item.name)}
		>
			{item.name}
			<p class={selected === item.name ? '' : 'hidden'}>
				{item.text}
			</p>
		</li>
	{/each}
</ul>

<!-- svelte-ignore css-unused-selector -->
<style lang="scss">
	h1 {
		padding: 10vh 0 5vh 6vw;
		width: fit-content;
		position: flex;
		font-size: var(--f_lg);
	}

	h3 {
		padding: 10vh 0 5vh 15vw;
	}

	workforce {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 1%;

		.img_Face {
			img {
				width: 60%;
				margin: 0 20%;
			}
		}
	}

	.affiliates {
		display: grid;
		grid-template-columns: 1fr 1fr 1fr 1fr;
		list-style-type: none;
		width: 80vw;
		margin: 10vw;

		.selected {
			border: var(--bord);
			border-radius: var(--rad);
			background-color: var(--back_Alt);
			color: var(--back_Main);
		}

		.unselected {
			height: fit-content;
		}

		li {
			background-color: var(--highlight);
			border: var(--bord);
			border-radius: var(--rad);
			font-size: var(--f_lg);
			cursor: pointer;
			width: fit-content;
			padding: 1%;
			margin: 2vh auto;

			p {
				font-size: var(--font);
				padding: 0;
				margin: 5% 0;
				cursor: default;
			}
		}

		.hidden {
			display: none;
		}
	}

	@media only screen and (min-width: 980px) {
		h1,
		h2 {
			padding: 18vh 0 5vh 46vw;
			width: fit-content;
			position: flex;
		}
	}

	@media only screen and (min-width: 1280px) {
		h1,
		h2 {
			font-size: var(--f_xl);
		}

		img_Intro {
			display: grid;
			grid-template-columns: 1fr 1fr;

			img {
				height: 100vh;
			}

			.text_Box {
				width: 40vw;
				margin: 20vh 2vw;
			}
		}

		.text_Block {
			.backBack {
				width: 100vw;
				height: 110vh;
				object-fit: cover;
			}
		}

		.overLay {
			margin-top: -60vh;
		}
	}
</style>
