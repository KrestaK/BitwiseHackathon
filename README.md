# BitwiseHackathon

<!DOCTYPE html>
<html data-ng-app>
    <head>
	<meta charset="UTF-8" />
        <title>Kresta's SuperCoolApp Voting System</title>
		<link rel="stylesheet" type="text/css" href="KrestaStyles.css"/>
        <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/angularjs/1.0.7/angular.min.js"></script>
        
    </head>
    <body>
	<form id="mainForm" name="mainForm">
	
	<header>
		<h1 align="center">Feature Voting for SuperCoolApp</h1>
		<h2 align="center">Please tell us which features you would love to see</h2>
		<br />
		<br />
	</header>
	
	<!--Post the voting results-->
		<div id='overallResults'>
		<h4>Voting Results:</h4>
		</div>
		<script type="text/javascript">document.write(mainForm.tallyForm());</script>
        
		
		<!--Feature #1: Login with FaceBook-->
		
		<div id='feature1'>
            <form data-ng-controller="SimpleController">
                <h4>Feature #1: Login with FaceBook</h4>
				
				
				<!--Radio Buttons for Upvote or Downvote-->
				<form data-ng-controller="RadioVoteController">
					Your Vote:
					<br />				
					<!--<input type="radio" value="up" data-ng-model="RadioVoteController" data-ng-value="true"/>Upvote<br />
					<input type="radio" value="down" data-ng-model="RadioVoteController" data-ng-value="false"/>Downvote<br />
					<div>You have currently selected: {{ RadioVoteController.value}} </div>-->
					
					<input type="radio" name="f1UpVote" data-ng-model="feature1Vote" value="up"/>Upvote<br />
					<input type="radio" name="f1DownVote" data-ng-model="feature1Vote" value="down"/>Downvote<br />
					<br />
					<button data-ng-click="tallyForm(); " value="Submit" onclick="alert('Thank you for your vote!');">Submit Vote</button>
					</form>
					
									
				<!--Comment Section -->	
                <form data-ng-controller="SimpleController">
					<br />
					Comments:
                    <textarea data-ng-model="featureComment" placeholder="Your Comment Here" style='width:450px'></textarea>
                    <button data-ng-click='addComment();' style='margin-top:10px;'>Post Comment</button>

                    <h4>Comments</h4>
                    <ul>
                        <li data-ng-repeat="comt in comment"> {{ comt }} </li>
                    </ul>
                </form> 
			</form>	
        </div>

		
		<!--Feature #2: Display the user's twitter feed-->
		
		<div id='feature2'>
            <form data-ng-controller="SimpleController">
                <h4>Feature #2: Display the user's twitter feed</h4>
				
				
				<!--Radio Buttons for Upvote or Downvote-->
				<form data-ng-controller="RadioVoteController">
					Your Vote:
					<br />				
					<input type="radio" name="f2UpVote" data-ng-model="feature2Vote" value="up"/>Upvote<br />
					<input type="radio" name="f2DownVote" data-ng-model="feature2Vote" value="down"/>Downvote<br />
					<br />
					<button data-ng-click="tallyForm(); " value="Submit" onclick="alert('Thank you for your vote!');">Submit Vote</button>
					</form>
					
									
				<!--Comment Section -->	
                <form data-ng-controller="SimpleController">
					<br />
					Comments:
                    <textarea data-ng-model="featureComment" placeholder="Your Comment Here" style='width:450px'></textarea>
                    <button data-ng-click='addComment();' style='margin-top:10px;'>Post Comment</button>

                    <h4>Comments</h4>
                    <ul>
                        <li data-ng-repeat="comt in comment"> {{ comt }} </li>
                    </ul>
                </form> 
			</form>	
        </div>
		
		
		<!--Feature #3: Threaded comments-->
		
		<div id='feature3'>
            <form data-ng-controller="SimpleController">
                <h4>Feature #3: Threaded comments</h4>
				
				<!--Radio Buttons for Upvote or Downvote-->
				<form data-ng-controller="RadioVoteController">
					Your Vote:
					<br />				
					<input type="radio" name="f3UpVote" data-ng-model="feature3Vote" value="up"/>Upvote<br />
					<input type="radio" name="f3DownVote" data-ng-model="feature3Vote" value="down"/>Downvote<br />
					<br />
					<button data-ng-click="tallyForm(); " value="Submit" onclick="alert('Thank you for your vote!');">Submit Vote</button>
					</form>
					
									
				<!--Comment Section -->	
                <form data-ng-controller="SimpleController">
					<br />
					Comments:
                    <textarea data-ng-model="featureComment" placeholder="Your Comment Here" style='width:450px'></textarea>
                    <button data-ng-click='addComment();' style='margin-top:10px;'>Post Comment</button>

                    <h4>Comments</h4>
                    <ul>
                        <li data-ng-repeat="comt in comment"> {{ comt }} </li>
                    </ul>
                </form> 
			</form>	
        </div>
		
		
		<!--Feature #4: Today's weather drawn from the weather.com API and displayed according to the user's zip code-->
		
		<div id='feature4'>
            <form data-ng-controller="SimpleController">
                <h4>Feature #4: Today's weather drawn from the weather.com API and displayed according to the user's zip code</h4>
				
				<!--Radio Buttons for Upvote or Downvote-->
				<form data-ng-controller="RadioVoteController">
					Your Vote:
					<br />				
					<input type="radio" name="f4UpVote" data-ng-model="feature4Vote" value="up"/>Upvote<br />
					<input type="radio" name="f4DownVote" data-ng-model="feature4Vote" value="down"/>Downvote<br />
					<br />
					<button data-ng-click="tallyForm(); " value="Submit" onclick="alert('Thank you for your vote!');">Submit Vote</button>
					</form>
					
									
				<!--Comment Section -->	
                <form data-ng-controller="SimpleController">
					<br />
					Comments:
                    <textarea data-ng-model="featureComment" placeholder="Your Comment Here" style='width:450px'></textarea>
                    <button data-ng-click='addComment();' style='margin-top:10px;'>Post Comment</button>

                    <h4>Comments</h4>
                    <ul>
                        <li data-ng-repeat="comt in comment"> {{ comt }} </li>
                    </ul>
                </form> 
			</form>	
        </div>
		
		
		<!--Feature #5: The ability to upload a profile picture-->
		
		<div id='feature5'>
            <form data-ng-controller="SimpleController">
                <h4>Feature #5: The ability to upload a profile picture</h4>
				
				<!--Radio Buttons for Upvote or Downvote-->
				<form data-ng-controller="RadioVoteController">
					Your Vote:
					<br />				
					<input type="radio" name="f5UpVote" data-ng-model="feature5Vote" value="up"/>Upvote<br />
					<input type="radio" name="f5DownVote" data-ng-model="feature5Vote" value="down"/>Downvote<br />
					<br />
					<button data-ng-click="tallyForm(); " value="Submit" onclick="alert('Thank you for your vote!');">Submit Vote</button>
					</form>
					
									
				<!--Comment Section -->	
                <form data-ng-controller="SimpleController">
					<br />
					Comments:
                    <textarea data-ng-model="featureComment" placeholder="Your Comment Here" style='width:450px'></textarea>
                    <button data-ng-click='addComment();' style='margin-top:10px;'>Post Comment</button>

                    <h4>Comments</h4>
                    <ul>
                        <li data-ng-repeat="comt in comment"> {{ comt }} </li>
                    </ul>
                </form> 
			</form>	
        </div>
	</form>	
				
		
		<script type="text/javascript">
			function voteController($scope){
				$scopes.votes = [];
				$scope.addVote = function(){
					if($scope.featureVote != ''){
						$scope.votes.push($scope.featureVote);
						$scope.featureVote = "";
					}
				}
			}
			
			function tallyForm(mainForm){
				var f1Results = 4;
				var f2Results = 2;
				var f3Results = 0;
				var f4Results = 1;
				var f5Results = 0;
				var votingResults = [];
				votingResults[0] = f1Results;
				votingResults[1] = f2Results;
				votingResults[2] = f3Results;
				votingResults[3] = f4Results;
				votingResults[4] = f5Results;
				
				for(var i = 0; i < mainForm.elements.length; i++){
					switch(name){
						case f1UpVote:
							f1Results ++;
							break;
						case f2UpVoteUp:
							f2Results ++;
							break;
						case f3UpVote:
							f3Results ++;
							break;
						case f4UpVote:
							f4Results ++;
							break;
						case f5UpVote:
							f5Results ++;
							break;
						default:
					}					
				}
				
				
				var orderedVotingResults = votingResults.sort();
				document.write("Voting Results: <br />");
				
				for(index in orderedVotingResults){
					document.write(orderedVotingResults[index] + "<br />");
				}
				
			}
			
			function CountController($scope){
				
				var f1Results = 4;
				var f2Results = 2;
				var f3Results = 0;
				var f4Results = 1;
				var f5Results = 0;
				var votingResults = [f1Results, f2Results, f3Results, f4Results, f5Results];

				
				for(var i = 0; i < form.elements.length; i++){
					if(form.elements[i].name == 'f1UpVote'){
						f1Results ++;
					}
				}
				
				for(var i = 0; i < form.elements.length; i++){
					if(form.elements[i].name == 'f2UpVoteUpVote'){
						f2Results ++;
					}
				}
				
				for(var i = 0; i < form.elements.length; i++){
					if(form.elements[i].name == 'f3UpVote'){
						f3Results ++;
					}
				}
				
				for(var i = 0; i < form.elements.length; i++){
					if(form.elements[i].name == 'f4UpVote'){
						f4Results ++;
					}
				}
				
				for(var i = 0; i < form.elements.length; i++){
					if(form.elements[i].name == 'f5UpVote'){
						f5Results ++;
					}
				}
				
				
				var orderedVotingResults = votingResults.sort();
				document.write("Voting Results: <br />");
				for(index in orderedVotingResults){
					document.write(orderedVotingResults[index] + "<br>");
				}
			}
		</script>
		
		
		
		
        <script type="text/javascript">
            function SimpleController($scope) {
                $scope.comment = [];
                $scope.addComment = function() {
                    if($scope.featureComment !=''){
                    $scope.comment.push($scope.featureComment);
                    $scope.featureComment = "";
                    }
                }

            }
			
        </script>
		
		<!--Weather API
		<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.5.1/jquery.min.js"></script>

		<script>
			jQuery(document).ready(function($) {
				$.ajax({
				url : "http://api.wunderground.com/api/111dfb5466361030/geolookup/conditions/q/IA/Cedar_Rapids.json",
				dataType : "jsonp",
				success : function(parsed_json) {
					var location = parsed_json['location']['city'];
					var temp_f = parsed_json['current_observation']['temp_f'];
					alert("Current temperature in " + location + " is: " + temp_f);
					}
				});
			});
		</script>-->
    </body>
</html>

<!--KrestaStyles.css-->
#feature1			{border:1px solid #DBDCE9;  float: center;	margin-left:auto; margin-right:auto;  width:550px; border-radius:7px;   padding: 25px; }
			
#feature2			{border:1px solid #DBDCE9;  float: center;	margin-left:auto; margin-right:auto;  width:550px; border-radius:7px;   padding: 25px; }

#feature3			{border:1px solid #DBDCE9;  float: center;	margin-left:auto; margin-right:auto;  width:550px; border-radius:7px;   padding: 25px; }

#feature4			{border:1px solid #DBDCE9;  float: center;	margin-left:auto; margin-right:auto;  width:550px; border-radius:7px;   padding: 25px; }

#feature5			{border:1px solid #DBDCE9;  float: center;	margin-left:auto; margin-right:auto;  width:550px; border-radius:7px;   padding: 25px; }

#overallResults		{border:1px solid #DBDCE9;  float: left; width:350px;	border-radius:7px;   padding: 15px; }

header				{font-family: Verdana, Arial;}

body				{font-family: Verdana, Arial; background-color: #ffffe5;}

div 					{width: 200px;}

h2 					{font: 400 40px/1.5 font-family: Verdana, Arial; margin: 0; padding: 0; }

ul 					{list-style-type: none;  margin: 0;padding: 0;}

li 					{font: 200 20px/1.5 font-family: Verdana, Arial; border-bottom: 1px solid #ccc;}

li a 					{text-decoration: none; color: #000; display: block;}
