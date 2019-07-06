---
layout: post
title: "A quick survey to find if you suffer from Impostor Syndrome"
date: 2016-12-28
---

<head>
	<style>
		footer {
		    border-top: 1px solid #d5d5d5;
		    font-size: .8em;
		}
		table{
			border: 3px;
			border-spacing: 2px;
			padding: 2px;
		}
		.evenrow {
			 background-color: #C4BCBC;
		}
		.oddrow {
			 background-color: #9099A2;
		}
		td {
		    font-size: 0.75em;
		    font-family:'Helvetica', 'Arial', 'Sans-Serif';
		    color: #000000;
		    height:30px;
		}
	</style>
	
	<title>A Survey to check if you suffer from Impostor Syndrome</title>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>
	<script type="text/javascript">
		function evaluateResults()
		{
			$(document).ready(function(){
				let sum = getSum();
				let message = getMessage(sum);

				if (message)
				{
					$("#result").html("<h2 class='results'> RESULT - Your score is "+sum+", "+message+"<h2>");
				}
			});
			
		};

		function getMessage(sum){
			let message;

			if(sum <= 40)
			{
				message = "You have a confident personality and have very few Impostor Syndrome charecteristics";
			} else if (sum >= 41 && sum <= 60) {
				message = "You have moderate Impostor Syndrome charecteristics and experiences";
			} else if (sum >= 61 && sum <= 80) {
				message = "You have frequent Impostor feelings which hamper your working style";
			} else if (sum >= 81 && sum <= 100) {
				message = "You have intense impostor feelings whcih frequently interfere with your career and life";
			}

			return message;
		};
		
		function getSum(){
			let sum = 0;
			for (let i = 1; i <= 20; i++) 
			{
				sum += parseInt($('input[name=q'+i+']:checked').val(), 10);
			}
			return sum;
		};
	</script>
</head>
<body>
<p>The <a href="http://paulineroseclance.com/pdf/IPscoringtest.pdf">Impostor Test</a> was developed to help individuals determine whether or not they have IP characteristics and, if so, to what
extent they are suffering.<br>
The code for this can be found at my github <a href='https://github.com/vighy/MemesAndSurveys'>repository location</a><p>

	<div id="result"><h2>...<h2>
	<div>
	<table>
		<tr class="oddrow">
			<td colspan="5">1. I have often succeeded on a test or task even though I was afraid that I would not do well before I undertook the task</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q1" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q1" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q1" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q1" value="4">4 (Often)</td>
			<td><input type="radio" name="q1" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">2. I can give the impression that I’m more competent than I really am</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q2" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q2" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q2" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q2" value="4">4 (Often)</td>
			<td><input type="radio" name="q2" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">3. I avoid evaluations if possible and have a dread of others evaluating me</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q3" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q3" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q3" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q3" value="4">4 (Often)</td>
			<td><input type="radio" name="q3" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">4. When people praise me for something I’ve accomplished, I’m afraid I won’t be able to live up to their expectations of me in the future</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q4" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q4" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q4" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q4" value="4">4 (Often)</td>
			<td><input type="radio" name="q4" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">5. I sometimes think I obtained my present position or gained my present success because I happened to be in the right place at the right time or knew the right people</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q5" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q5" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q5" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q5" value="4">4 (Often)</td>
			<td><input type="radio" name="q5" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">6. I’m afraid people important to me may find out that I’m not as capable as they think I am</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q6" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q6" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q6" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q6" value="4">4 (Often)</td>
			<td><input type="radio" name="q6" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">7. I tend to remember the incidents in which I have not done my best more than those times I have done my best</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q7" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q7" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q7" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q7" value="4">4 (Often)</td>
			<td><input type="radio" name="q7" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">8. I rarely do a project or task as well as I’d like to do it</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q8" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q8" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q8" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q8" value="4">4 (Often)</td>
			<td><input type="radio" name="q8" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">9. Sometimes I feel or believe that my success in my life or in my job has been the result of some kind of error</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q9" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q9" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q9" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q9" value="4">4 (Often)</td>
			<td><input type="radio" name="q9" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">10. It’s hard for me to accept compliments or praise about my intelligence or accomplishments</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q10" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q10" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q10" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q10" value="4">4 (Often)</td>
			<td><input type="radio" name="q10" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">11. At times, I feel my success has been due to some kind of luck</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q11" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q11" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q11" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q11" value="4">4 (Often)</td>
			<td><input type="radio" name="q11" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">12. I’m disappointed at times in my present accomplishments and think I should have accomplished much more</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q12" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q12" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q12" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q12" value="4">4 (Often)</td>
			<td><input type="radio" name="q12" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">13. Sometimes I’m afraid others will discover how much knowledge or ability I really lack</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q13" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q13" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q13" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q13" value="4">4 (Often)</td>
			<td><input type="radio" name="q13" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">14. I’m often afraid that I may fail at a new assignment or undertaking even though I generally do well at what I attempt</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q14" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q14" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q14" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q14" value="4">4 (Often)</td>
			<td><input type="radio" name="q14" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">15. When I’ve succeeded at something and received recognition for my accomplishments, I have doubts that I can keep repeating that success</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q15" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q15" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q15" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q15" value="4">4 (Often)</td>
			<td><input type="radio" name="q15" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">16. If I receive a great deal of praise and recognition for something I’ve accomplished, I tend to discount the importance of what I’ve done</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q16" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q16" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q16" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q16" value="4">4 (Often)</td>
			<td><input type="radio" name="q16" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">17. I often compare my ability to those around me and think they may be more intelligent than I am</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q17" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q17" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q17" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q17" value="4">4 (Often)</td>
			<td><input type="radio" name="q17" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">18. I often worry about not succeeding with a project or examination, even though others around me have considerable confidence that I will do well</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q18" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q18" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q18" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q18" value="4">4 (Often)</td>
			<td><input type="radio" name="q18" value="5">5 (Very True)</td>
		</tr>
		<tr class="oddrow">
			<td colspan="5">19. If I’m going to receive a promotion or gain recognition of some kind, I hesitate to tell others until it is an accomplished fact</td>
		</tr>
		<tr class="oddrow">	
			<td><input type="radio" name="q19" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q19" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q19" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q19" value="4">4 (Often)</td>
			<td><input type="radio" name="q19" value="5">5 (Very True)</td>
		</tr>
		<tr class="evenrow">
			<td colspan="5">20. I feel bad and discouraged if I’m not “the best” or at least “very special” in situations that involve achievement</td>
		</tr>
		<tr class="evenrow">	
			<td><input type="radio" name="q20" value="1">1 (Not at all True)</td>
			<td><input type="radio" name="q20" value="2">2 (Rarely)</td>
			<td><input type="radio" name="q20" value="3">3 (Sometimes)</td>
			<td><input type="radio" name="q20" value="4">4 (Often)</td>
			<td><input type="radio" name="q20" value="5">5 (Very True)</td>
		</tr>
	</table>
	</div>
	<button onclick="evaluateResults();">Submit</button>

