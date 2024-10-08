<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
	import { onMount } from 'svelte';
	let daysleft;
	onMount(() => {
        // Set the date we're counting down to
        var countDownDate = new Date("Nov 5, 2024").getTime();

        // Update the count down every 1 second
        var x = setInterval(function() {

            // Get today's date and time
            var now = new Date().getTime();

            // Find the distance between now and the count down date
            var distance = countDownDate - now;

            // Time calculations for days, hours, minutes and seconds
            var days = Math.floor(distance / (1000 * 60 * 60 * 24));

            // Display the result in the element with id="countdown"
            daysleft.innerHTML = days;

            // If the count down is finished, write some text
        }, 1000);
	})

</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="live">
	<h2>
		Live from the Campaign Kickoff:
	</h2>
	<img src="https://static.wixstatic.com/media/0f7e9e_6092b52891934fecaf57b4b19bada504f000.jpg/v1/fill/w_392,h_502,al_c,q_80,usm_0.33_1.00_0.00,enc_auto/0f7e9e_6092b52891934fecaf57b4b19bada504f000.jpg" alt="" style="width: 392px; height: 502px; object-fit: cover; object-position: 50% 50%;" width="392" height="502" data-ssr-src-done="true" fetchpriority="high">

</section>
<section>
<div class="daysTicker">
<div class="highlight">Days until Election Day</div>
<p bind:this={daysleft}></p>
</div>
<div class = "about">
<h3>
Economist | Lawyer | Policymaker <br/>
Parent of 4 PAUSD Students
PTA President (2022-24)
</h3>
<h1 class="super">
ROWENA CHIU
</h1><h2>
for Palo Alto
School Board
</h2>
</div>
</section>
<div class="grey">
<div class="statement">
<h1>
Candidate Statement
</h1>
<div>
I'm running for PAUSD School Board, because I care deeply about providing a choice and voice for those who feel underrepresented, as well as a high-quality education for all PAUSD students.

 

With four children in PAUSD (10th Grade at Middle College, 7th Grade at JLS, 4th & 1st Grade at Ohlone), and having served as JLS Connections Board President and Ohlone PTA President, I have both deep knowledge about the complexities and passion for the potential within PAUSD.

 

I also have both the academic and professional experience to understand the challenges in PAUSD and to make an impact. I have a BA in English Literature, MA in English Literature, MBA in Corporate Finance, Postgraduate Diploma in Law, Legal Practice Course, MSc in International Management For China, and PhD in Anthropology & Culture (incomplete). Additionally, I have worked in the fields of business, economics, law, and management consulting for top corporations such as Accenture, PricewaterhouseCoopers, McKinsey & Company, as well as the World Bank.
</div>
</div>
</div>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
.statement{
	width:30vw;
	
	padding:50px;
	padding-left:10vw;
}
.about {
	margin-top:10px;
	width:30vw;
	margin-left:0px
}
.grey{
	position: relative;
  left: 50%;
	width:100vw;
	margin-bottom:-20px;
  transform: translateX(-50%);
	background:#383838;
	color:white;
}
	.live {
		width:80vw;
		position: relative;
  left: 50%;
  transform: translateX(-50%);
		background-color: #f5f5f5;
		padding:10px;
		margin:10px;
	}
	section{
		width:80vw;
		position: relative;
  left: 50%;
  transform: translateX(-50%);
		padding:100px;
		margin:10px;
	}
	p {
		margin:10px;
		padding:0px;
		font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: normal;
	font-size:20px;
	color:rgb(5,5,5);
	}
	.super {
		font-family: "Poppins", sans-serif;
  font-weight: 700;
  font-style: normal;
	font-size:100px;
	line-height: 90%;
	margin:0px;
	margin-left:-15px;
letter-spacing: 3px;
	}
	h2{
		font-family: "Poppins", sans-serif;
  font-weight: 400;
  font-style: normal;
	font-size:40px;
	margin-top:0px;
	}
	h1 {
	font-family: "Poppins", sans-serif;
  font-weight: 700;
  font-style: normal;
	font-size:40px;
	margin-top:0px;
	width:auto;
	margin-left:-10px;
	height:fit-content;
	
	padding:10px;
	text-align: left;
	}

	.welcome {
	}
	.highlight{
		padding:10px;
		background:#e03539;
		color:white;
		font-family: "Poppins", sans-serif;
  font-weight: 700;
  font-style: normal;
	font-size:20px;
	width: fit-content;
	}
	.daysTicker{
		display:flex;
	}
</style>
