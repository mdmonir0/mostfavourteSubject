# mostfavourteSubject
 problem-solving


 ### mostfavourteSubject 
 problem-solving


$students = [
    [
        'name' => 'Monir',
        'age' => '26',
        'subjects' => ['database, algorithom'],
    ],
    [
        'name' => 'kaium',
        'age' => '28',
        'subjects' => ['database, mathematics'],
    ],
    [
        'name' => 'Robin',
        'age' => '27',
        'subjects' => ['database, phyysics'],
    ],
];



##loop

function mostFavourteSubject($students): string
{
 
    $subjects= [];

    foreach( $students as $student){

        foreach($student['subjects'] as $subject){

            if(isset($subjects['$subject'])){
                $subjects[$subject] += 1;
            }
            if(!isset($subjects['$`subject'])){
                $subjects[$subject] = 1;
            }
        }
    }

    $subjects = array_flip($subjects);
    return end($subjects);

}
mostFavourteSubject($students);



````php````

## output 

"database"


