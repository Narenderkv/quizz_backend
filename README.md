# quizz_backend
npm i
npm start

import  db in phpmyadmin file already share

Sample data 


http://localhost:3000/register
{
"email":"narender@gmail.com",
"name":"narender",
"password":"1231230"
}

http://localhost:3000/login

{
"email":"narender@gmail.com",
"password":"1231230"
}

http://localhost:3000/add_quizzes
{
  "user_id":"1", //for identify the  user quizz
  "title": "My Quiz",
  "questions": [
    {
      "question": "Question 1",
      "answer": ["Answer 1", "Answer 2", "Answer 3"],
      "correct_ans":"Answer 1"
    },
    {
      "question": "Question 2",
      "answer": ["Answer 4", "Answer 5", "Answer 6"],
      "correct_ans":"Answer 5"
    },
    {
      "question": "Question 3",
      "answer": ["Answer 7", "Answer 8", "Answer 9"],
      "correct_ans":"Answer 9"
    }
  ]
}

http://localhost:3000/user_quizzes

Login user quizz

{
    "id":"1"
}

http://localhost:3000/attempt_quiz
{
  "id":"41", 
  "user_id":"1",  //if user_id is match with quizz created user then update the score and status
  "questions": [
    {
      "question": "Question 1",
      "answer":"Answer 1"
    },
    {
      "question": "Question 2",
      "answer":"Answer 5"
    },
    {
      "question": "Question 3",
      "answer":"Answer 9"
    }
  ]
}

http://localhost:3000/all_quiz

get all quiz


