<h1 align="center">
  Hi, Nice to Meet You! <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px">
</h1>

<p align="center">   
  <a href="mailto:fernandozanner@gmail.com" target="_blank"><img src="https://img.shields.io/badge/-Email-0D1117?style=for-the-badge&logo=gmail&logoColor=0078D4"></a>
  <a href="https://www.linkedin.com/in/fernandozanner/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=0078D4"></a>
    <!--https://dev.to/envoy_/150-badges-for-github-pnk-->
</p>

## 🏋 About Me

```php
<?php
namespace WhoIAm;

use /A/Lot/Of/Enthusiasm;

/**
 * That's me
**/
class Me 
{

  private $name = 'Fernando Zanner';
  protected $alias = '@zannerfkw';
  protected $languageSpoken;
  protected $skills = [];
  protected $graduated = ['Systems Analyst and Developer', 'Software Engineering', 'IT Security'];
  protected $role = ['Information Security and Data Protection Analyst'];
  
  private $jobs = array(  
    'Full Stack Developer', 
    'Full Stack PHP',
    'Software Engineering',
    'Software Architect',
    'Systems Analyst'
  );

  public function __construct() 
  {
      $this->languageSpoken = ['pt_BR', 'en_US'];
      $this->setSkill( [ 
                        'PHP', 
                        'python', 
                        'Bootstrap', 
                        'MySql', 
                        'Laravel', 
                        'Vue.js', 
                        'Javascript', 
                        'Docker', 
                        'innertia.js', 
                        'Composer', 
                        'Git', 
                        'Linux' 
                      ] );
  }
  
  private function setSkill(string|array $skill) : void
  {
      if ( is_array($skill) )
          $this->skills = array_merge( $this->skills, $skill);
      else
          $this->skills[] = $skill;
  }
  
  protected function searchJob(string $jobRole) : bool
  {
      return ( in_array($jobRole, $this->jobs) ? true : false );
  }
  
  public function addWork(string $workRole) : string
  {
      if ( $this->searchJob($workRole) == true ) {
          array_push( $this->role, $workRole );
          return 'New job successfully added!';
      }
      
      return 'Unfortunately this job does not meet the ments.';
  }
  
  public function __toString()
  {
  	$message = "Hi i apreciate your time so let's make this quick, i am {$this->name}, ";
        $message .= "fluent in {$this->languageSpoken[0]} and i have technical understanding {$this->languageSpoken[1]}, ";
  	$message .= "currently work as {$this->role[0]} at the State Government of Santa Catarina - Brazil, ";
  	$message .= "and i'm looking for additional jobs that add value to my professional career as a software developer, ";
        $message .= "like {$this->role[1]}. \n";
  	$message .= "\nMy Skills: \n";
  	
  	foreach ( $this->skills as $index => $skill ) {
  		if ( $index === array_key_last($this->skills) ) 
  			$message .= "{$skill} and a lot of Enthusiasm =)\n";
  		else 
  			$message .= "{$skill}, ";
  	}
  	
  	$message .= "\nGraduations: \n";
  	
  	foreach ( $this->graduated as $graduated ) {
  		$message .= "{$graduated} \n";
  	}
  	
        $message .= "\n\nThanks for dropping by, hope you find interesting my profile :)\n";
  	$message .= "-> {$this->alias} follow-me on Instagram\n";
  	$message .= "My best regards.";
  	
  	return $message;
  }
  
 }

$me = new Me();
$me->addWork('Full Stack Developer');
print($me);
 
?>
```
```
Output:
Hi i apreciate your time so let's make this quick, i am Fernando Zanner, 
fluent in pt_BR and i have technical understanding en_US, currently work 
as Information Security and Data Protection Analyst at the State Government 
of Santa Catarina - Brazil, and i'm looking for additional jobs that add 
value to my professional career as a software developer, like Full Stack Developer. 

My Skills: 
PHP, python, Bootstrap, MySql, Laravel, Vue.js, Javascript, Docker, 
innertia.js, Composer, Git, Linux and a lot of Enthusiasm =)

Graduations: 
Systems Analyst and Developer 
Software Engineering 
IT Security 


Thanks for dropping by, hope you find interesting my profile :)
-> @zannerfkw follow-me on Instagram
My best regards.
```

## 📈 Github Stats

<div align="center">

  <div>
    <img alt="Fernando Zanner Github Stats" src="http://github-readme-streak-stats.herokuapp.com?user=FernandoZanner&theme=github-dark&hide_border=true&date_format=M%20j%5B%2C%20Y%5D&dates=FFFFFF&sideLabels=0078D4&currStreakLabel=0078D4&stroke=0078D4&ring=0078D4" />
  </div>

  <hr/>

  <div>
    <img alt="Fernando Zanner Contribution Graph" src="https://activity-graph.herokuapp.com/graph?username=FernandoZanner&bg_color=0D1117&color=0078D4&line=FFFFFF&point=0078D4&hide_border=true" />
  <div>

</div>

