# Day39
>DATA

Student absent and Submitting task in between 15Oct to 31 Oct 2020

/* 1 createdAt:4/8/2022, 4:09:05 PM*/

{
	"_id" : ObjectId("625010c97d8490d5270b4425"),
	"name" : "GGG",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-31",
	"problem_solved" : 12
},


{
	"_id" : ObjectId("625010bb7d8490d5270b4424"),
	"name" : "FFF",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-15",
	"problem_solved" : 67
},


{
	"_id" : ObjectId("625010a87d8490d5270b4423"),
	"name" : "EEE",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-10",
	"problem_solved" : 0
},

{
	"_id" : ObjectId("6250108c7d8490d5270b4422"),
	"name" : "DDD",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-18",
	"problem_solved" : 24
},


{
	"_id" : ObjectId("625010787d8490d5270b4421"),
	"name" : "CCC",
	"placement_attendence" : "A",
	"task_submission" : "2020-11-03",
	"problem_solved" : 0
},


{
	"_id" : ObjectId("625010407d8490d5270b4420"),
	"name" : "BBB",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-03",
	"problem_solved" : 81
},

{
	"_id" : ObjectId("6250102a7d8490d5270b441f"),
	"name" : "AAA",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-30",
	"problem_solved" : 18
}	Query: db.students.find({$and:[{placement_attendence:"A"} , {task_submission:{$gte: '2020-10-15' , $lte:'2020-10-31'}}]});



{
	"_id" : ObjectId("6250108c7d8490d5270b4422"),
	"name" : "DDD",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-18",
	"problem_solved" : 24
}


Student absent and Submitting task in between 15Oct to 31 Oct 2020

/* 1 createdAt:4/8/2022, 4:09:05 PM*/

{
	"_id" : ObjectId("625010c97d8490d5270b4425"),
	"name" : "GGG",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-31",
	"problem_solved" : 12
},

/* 2 createdAt:4/8/2022, 4:08:51 PM*/
{
	"_id" : ObjectId("625010bb7d8490d5270b4424"),
	"name" : "FFF",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-15",
	"problem_solved" : 67
},

/* 3 createdAt:4/8/2022, 4:08:32 PM*/
{
	"_id" : ObjectId("625010a87d8490d5270b4423"),
	"name" : "EEE",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-10",
	"problem_solved" : 0
},

/* 4 createdAt:4/8/2022, 4:08:04 PM*/
{
	"_id" : ObjectId("6250108c7d8490d5270b4422"),
	"name" : "DDD",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-18",
	"problem_solved" : 24
},

/* 5 createdAt:4/8/2022, 4:07:44 PM*/
{
	"_id" : ObjectId("625010787d8490d5270b4421"),
	"name" : "CCC",
	"placement_attendence" : "A",
	"task_submission" : "2020-11-03",
	"problem_solved" : 0
},

/* 6 createdAt:4/8/2022, 4:06:48 PM*/
{
	"_id" : ObjectId("625010407d8490d5270b4420"),
	"name" : "BBB",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-03",
	"problem_solved" : 81
},

/* 7 createdAt:4/8/2022, 4:06:26 PM*/
{
	"_id" : ObjectId("6250102a7d8490d5270b441f"),
	"name" : "AAA",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-30",
	"problem_solved" : 18
}	


Query:

db.students.find({$and:[{placement_attendence:"A"} , {task_submission:{$gte: '2020-10-15' , $lte:'2020-10-31'}}]});



{
	"_id" : ObjectId("6250108c7d8490d5270b4422"),
	"name" : "DDD",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-18",
	"problem_solved" : 24
}


2. Mentor with more than 15 mentee

/* 1 createdAt:4/8/2022, 6:22:29 PM*/
{
	"_id" : ObjectId("6250300d7d8490d5270b443e"),
	"mentor_name" : "M4",
	"mentees" : "45",
	"topic" : "Node.js"
},

/* 2 createdAt:4/8/2022, 6:22:12 PM*/
{
	"_id" : ObjectId("62502ffc7d8490d5270b443d"),
	"mentor_name" : "M3",
	"mentees" : "15",
	"topic" : "JS"
},

/* 3 createdAt:4/8/2022, 6:21:41 PM*/
{
	"_id" : ObjectId("62502fdd7d8490d5270b443c"),
	"mentor_name" : "M2",
	"mentees" : "3",
	"topic" : "DI"
},

/* 4 createdAt:4/8/2022, 6:21:19 PM*/
{
	"_id" : ObjectId("62502fc77d8490d5270b443b"),
	"mentor_name" : "M1",
	"mentees" : "12",
	"topic" : "HTML"
}	Query: db.mentors.find({mentees:{$gt:15}})


Output: 
{
	"_id" : ObjectId("6250300d7d8490d5270b443e"),
	"mentor_name" : "M4",
	"mentees" : 45,
	"topic" : "Node.js"
}


Query: db.mentors.find({mentees:{$gt:15}})


Output: 
{
	"_id" : ObjectId("6250300d7d8490d5270b443e"),
	"mentor_name" : "M4",
	"mentees" : 45,
	"topic" : "Node.js"
}


3. NO. of Problems solved by Each Student

/* 1 createdAt:4/8/2022, 4:09:05 PM*/
{
	"_id" : ObjectId("625010c97d8490d5270b4425"),
	"name" : "GGG",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-31",
	"problem_solved" : 12
},

/* 2 createdAt:4/8/2022, 4:08:51 PM*/
{
	"_id" : ObjectId("625010bb7d8490d5270b4424"),
	"name" : "FFF",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-15",
	"problem_solved" : 67
},

/* 3 createdAt:4/8/2022, 4:08:32 PM*/
{
	"_id" : ObjectId("625010a87d8490d5270b4423"),
	"name" : "EEE",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-10",
	"problem_solved" : 0
},

/* 4 createdAt:4/8/2022, 4:08:04 PM*/
{
	"_id" : ObjectId("6250108c7d8490d5270b4422"),
	"name" : "DDD",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-18",
	"problem_solved" : 24
},

/* 5 createdAt:4/8/2022, 4:07:44 PM*/
{
	"_id" : ObjectId("625010787d8490d5270b4421"),
	"name" : "CCC",
	"placement_attendence" : "A",
	"task_submission" : "2020-11-03",
	"problem_solved" : 0
},

/* 6 createdAt:4/8/2022, 4:06:48 PM*/
{
	"_id" : ObjectId("625010407d8490d5270b4420"),
	"name" : "BBB",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-03",
	"problem_solved" : 81
},

/* 7 createdAt:4/8/2022, 4:06:26 PM*/
{
	"_id" : ObjectId("6250102a7d8490d5270b441f"),
	"name" : "AAA",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-30",
	"problem_solved" : 18
}	Query: db.students.find({{"problem_solved":1,"name":1,_id:0}})
   

Output:
/* 1 */
{
	"name" : "AAA",
	"problem_solved" : 18
},

/* 2 */
{
	"name" : "BBB",
	"problem_solved" : 81
},

/* 3 */
{
	"name" : "CCC",
	"problem_solved" : 0
},

/* 4 */
{
	"name" : "DDD",
	"problem_solved" : 24
},

/* 5 */
{
	"name" : "EEE",
	"problem_solved" : 0
},

/* 6 */
{
	"name" : "FFF",
	"problem_solved" : 67
},

/* 7 */
{
	"name" : "GGG",
	"problem_solved" : 12
}

Query: db.students.find({{"problem_solved":1,"name":1,_id:0}})
   

Output:
/* 1 */
{
	"name" : "AAA",
	"problem_solved" : 18
},

/* 2 */
{
	"name" : "BBB",
	"problem_solved" : 81
},

/* 3 */
{
	"name" : "CCC",
	"problem_solved" : 0
},

/* 4 */
{
	"name" : "DDD",
	"problem_solved" : 24
},

/* 5 */
{
	"name" : "EEE",
	"problem_solved" : 0
},

/* 6 */
{
	"name" : "FFF",
	"problem_solved" : 67
},

/* 7 */
{
	"name" : "GGG",
	"problem_solved" : 12
}


4. Compnay drives between 15 october and 31 Ocy 2020

/* 1 createdAt:4/8/2022, 6:19:28 PM*/
{
	"_id" : ObjectId("62502f587d8490d5270b443a"),
	"company_name" : "WWW Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-10"
},

/* 2 createdAt:4/8/2022, 6:19:03 PM*/
{
	"_id" : ObjectId("62502f3f7d8490d5270b4439"),
	"company_name" : "UUU Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-14"
},

/* 3 createdAt:4/8/2022, 6:18:50 PM*/
{
	"_id" : ObjectId("62502f327d8490d5270b4438"),
	"company_name" : "VVV Enterprises",
	"placement_attendence" : "A",
	"company_visit" : "2020-10-15"
},

/* 4 createdAt:4/8/2022, 6:18:36 PM*/
{
	"_id" : ObjectId("62502f247d8490d5270b4437"),
	"company_name" : "ZZZ Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-16"
},

/* 5 createdAt:4/8/2022, 6:18:21 PM*/
{
	"_id" : ObjectId("62502f157d8490d5270b4436"),
	"company_name" : "YYY Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-11-6"
},

/* 6 createdAt:4/8/2022, 6:18:11 PM*/
{
	"_id" : ObjectId("62502f0b7d8490d5270b4435"),
	"company_name" : "XXX Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-6"
}	Query: db.company_drive.find({company_visit:{$gte: '2020-10-15' , $lte:'2020-10-31'}});

Output:
/* 1 createdAt:4/8/2022, 6:18:36 PM*/
{
	"_id" : ObjectId("62502f247d8490d5270b4437"),
	"company_name" : "ZZZ Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-16"
},

/* 2 createdAt:4/8/2022, 6:18:50 PM*/
{
	"_id" : ObjectId("62502f327d8490d5270b4438"),
	"company_name" : "VVV Enterprises",
	"placement_attendence" : "A",
	"company_visit" : "2020-10-15"
}


Query: db.company_drive.find({company_visit:{$gte: '2020-10-15' , $lte:'2020-10-31'}});

Output:
/* 1 createdAt:4/8/2022, 6:18:36 PM*/
{
	"_id" : ObjectId("62502f247d8490d5270b4437"),
	"company_name" : "ZZZ Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-16"
},

/* 2 createdAt:4/8/2022, 6:18:50 PM*/
{
	"_id" : ObjectId("62502f327d8490d5270b4438"),
	"company_name" : "VVV Enterprises",
	"placement_attendence" : "A",
	"company_visit" : "2020-10-15"
}


5.  Topics taught in October
/* 1 createdAt:4/8/2022, 5:17:53 PM*/
{
	"_id" : ObjectId("625020e97d8490d5270b4430"),
	"topic" : "HTML",
	"date" : "2020-08-15",
	"mentor" : "M1"
},

/* 2 createdAt:4/8/2022, 5:17:36 PM*/
{
	"_id" : ObjectId("625020d87d8490d5270b442f"),
	"topic" : "Node.js",
	"date" : "2020-08-05",
	"mentor" : "M4"
},

/* 3 createdAt:4/8/2022, 5:17:16 PM*/
{
	"_id" : ObjectId("625020c47d8490d5270b442e"),
	"topic" : "JS",
	"date" : "2020-10-15",
	"mentor" : "M3"
},

/* 4 createdAt:4/8/2022, 5:16:42 PM*/
{
	"_id" : ObjectId("625020a27d8490d5270b442d"),
	"topic" : "DI",
	"date" : "2020-10-03",
	"mentor" : "M2"
},

/* 5 createdAt:4/8/2022, 5:16:17 PM*/
{
	"_id" : ObjectId("625020897d8490d5270b442c"),
	"topic" : "React",
	"date" : "2020-12-30",
	"mentor" : "M1"
}	Query:
db.topics.find({date:{$gte: '2020-10-01' , $lte:'2020-10-31'}});

output:
/* 1 createdAt:4/8/2022, 5:16:42 PM*/
{
	"_id" : ObjectId("625020a27d8490d5270b442d"),
	"topic" : "DI",
	"date" : "2020-10-03",
	"mentor" : "M2"
},

/* 2 createdAt:4/8/2022, 5:17:16 PM*/
{
	"_id" : ObjectId("625020c47d8490d5270b442e"),
	"topic" : "JS",
	"date" : "2020-10-15",
	"mentor" : "M3"
}

Query:
db.topics.find({date:{$gte: '2020-10-01' , $lte:'2020-10-31'}});

output:
/* 1 createdAt:4/8/2022, 5:16:42 PM*/
{
	"_id" : ObjectId("625020a27d8490d5270b442d"),
	"topic" : "DI",
	"date" : "2020-10-03",
	"mentor" : "M2"
},

/* 2 createdAt:4/8/2022, 5:17:16 PM*/
{
	"_id" : ObjectId("625020c47d8490d5270b442e"),
	"topic" : "JS",
	"date" : "2020-10-15",
	"mentor" : "M3"
}


6.tasks taught in October

/* 1 createdAt:4/8/2022, 5:22:44 PM*/
{
	"_id" : ObjectId("6250220c7d8490d5270b4434"),
	"task_name" : "Promise Functionality",
	"submission_date" : "2020-12-19",
	"difficulty_level" : "Easy"
},

/* 2 createdAt:4/8/2022, 5:21:58 PM*/
{
	"_id" : ObjectId("625021de7d8490d5270b4433"),
	"task_name" : "Call Back Function",
	"submission_date" : "2020-10-19",
	"difficulty_level" : "Medium"
},

/* 3 createdAt:4/8/2022, 5:21:34 PM*/
{
	"_id" : ObjectId("625021c67d8490d5270b4432"),
	"task_name" : "Controlled Form",
	"submission_date" : "2020-11-09",
	"difficulty_level" : "Difficult"
},

/* 4 createdAt:4/8/2022, 5:20:54 PM*/
{
	"_id" : ObjectId("6250219e7d8490d5270b4431"),
	"task_name" : "Design Page",
	"submission_date" : "2020-10-09",
	"difficulty_level" : "Easy"
}			Query:
db.tasks.find({submission_date:{$gte: '2020-10-01' , $lte:'2020-10-31'}});

Output:

/* 1 createdAt:4/8/2022, 5:20:54 PM*/
{
	"_id" : ObjectId("6250219e7d8490d5270b4431"),
	"task_name" : "Design Page",
	"submission_date" : "2020-10-09",
	"difficulty_level" : "Easy"
},

/* 2 createdAt:4/8/2022, 5:21:58 PM*/
{
	"_id" : ObjectId("625021de7d8490d5270b4433"),
	"task_name" : "Call Back Function",
	"submission_date" : "2020-10-19",
	"difficulty_level" : "Medium"
}


Query:
db.tasks.find({submission_date:{$gte: '2020-10-01' , $lte:'2020-10-31'}});

Output:

/* 1 createdAt:4/8/2022, 5:20:54 PM*/
{
	"_id" : ObjectId("6250219e7d8490d5270b4431"),
	"task_name" : "Design Page",
	"submission_date" : "2020-10-09",
	"difficulty_level" : "Easy"
},

/* 2 createdAt:4/8/2022, 5:21:58 PM*/
{
	"_id" : ObjectId("625021de7d8490d5270b4433"),
	"task_name" : "Call Back Function",
	"submission_date" : "2020-10-19",
	"difficulty_level" : "Medium"
}


7. Company Drives appeared for Placement

/* 1 createdAt:4/8/2022, 6:19:28 PM*/
{
	"_id" : ObjectId("62502f587d8490d5270b443a"),
	"company_name" : "WWW Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-10"
},

/* 2 createdAt:4/8/2022, 6:19:03 PM*/
{
	"_id" : ObjectId("62502f3f7d8490d5270b4439"),
	"company_name" : "UUU Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-14"
},

/* 3 createdAt:4/8/2022, 6:18:50 PM*/
{
	"_id" : ObjectId("62502f327d8490d5270b4438"),
	"company_name" : "VVV Enterprises",
	"placement_attendence" : "A",
	"company_visit" : "2020-10-15"
},

/* 4 createdAt:4/8/2022, 6:18:36 PM*/
{
	"_id" : ObjectId("62502f247d8490d5270b4437"),
	"company_name" : "ZZZ Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-16"
},

/* 5 createdAt:4/8/2022, 6:18:21 PM*/
{
	"_id" : ObjectId("62502f157d8490d5270b4436"),
	"company_name" : "YYY Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-11-6"
},

/* 6 createdAt:4/8/2022, 6:18:11 PM*/
{
	"_id" : ObjectId("62502f0b7d8490d5270b4435"),
	"company_name" : "XXX Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-6"
}	Query:
db.company_drive.find({placement_attendence:'P'})
   

Output:
/* 1 createdAt:4/8/2022, 6:18:11 PM*/
{
	"_id" : ObjectId("62502f0b7d8490d5270b4435"),
	"company_name" : "XXX Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-6"
},

/* 2 createdAt:4/8/2022, 6:18:21 PM*/
{
	"_id" : ObjectId("62502f157d8490d5270b4436"),
	"company_name" : "YYY Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-11-6"
},

/* 3 createdAt:4/8/2022, 6:18:36 PM*/
{
	"_id" : ObjectId("62502f247d8490d5270b4437"),
	"company_name" : "ZZZ Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-16"
},

/* 4 createdAt:4/8/2022, 6:19:03 PM*/
{
	"_id" : ObjectId("62502f3f7d8490d5270b4439"),
	"company_name" : "UUU Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-14"
},

/* 5 createdAt:4/8/2022, 6:19:28 PM*/
{
	"_id" : ObjectId("62502f587d8490d5270b443a"),
	"company_name" : "WWW Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-10"
}


7. Company Drives appeared for Placement

/* 1 createdAt:4/8/2022, 6:19:28 PM*/
{
	"_id" : ObjectId("62502f587d8490d5270b443a"),
	"company_name" : "WWW Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-10"
},

/* 2 createdAt:4/8/2022, 6:19:03 PM*/
{
	"_id" : ObjectId("62502f3f7d8490d5270b4439"),
	"company_name" : "UUU Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-14"
},

/* 3 createdAt:4/8/2022, 6:18:50 PM*/
{
	"_id" : ObjectId("62502f327d8490d5270b4438"),
	"company_name" : "VVV Enterprises",
	"placement_attendence" : "A",
	"company_visit" : "2020-10-15"
},

/* 4 createdAt:4/8/2022, 6:18:36 PM*/
{
	"_id" : ObjectId("62502f247d8490d5270b4437"),
	"company_name" : "ZZZ Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-16"
},

/* 5 createdAt:4/8/2022, 6:18:21 PM*/
{
	"_id" : ObjectId("62502f157d8490d5270b4436"),
	"company_name" : "YYY Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-11-6"
},

/* 6 createdAt:4/8/2022, 6:18:11 PM*/
{
	"_id" : ObjectId("62502f0b7d8490d5270b4435"),
	"company_name" : "XXX Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-6"
}	Query:
db.company_drive.find({placement_attendence:'P'})
   

Output:
/* 1 createdAt:4/8/2022, 6:18:11 PM*/
{
	"_id" : ObjectId("62502f0b7d8490d5270b4435"),
	"company_name" : "XXX Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-6"
},

/* 2 createdAt:4/8/2022, 6:18:21 PM*/
{
	"_id" : ObjectId("62502f157d8490d5270b4436"),
	"company_name" : "YYY Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-11-6"
},

/* 3 createdAt:4/8/2022, 6:18:36 PM*/
{
	"_id" : ObjectId("62502f247d8490d5270b4437"),
	"company_name" : "ZZZ Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-16"
},

/* 4 createdAt:4/8/2022, 6:19:03 PM*/
{
	"_id" : ObjectId("62502f3f7d8490d5270b4439"),
	"company_name" : "UUU Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-14"
},

/* 5 createdAt:4/8/2022, 6:19:28 PM*/
{
	"_id" : ObjectId("62502f587d8490d5270b443a"),
	"company_name" : "WWW Enterprises",
	"placement_attendence" : "P",
	"company_visit" : "2020-10-10"
}


8. Placement attended by Students

/* 1 createdAt:4/8/2022, 4:09:05 PM*/
{
	"_id" : ObjectId("625010c97d8490d5270b4425"),
	"name" : "GGG",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-31",
	"problem_solved" : 12
},

/* 2 createdAt:4/8/2022, 4:08:51 PM*/
{
	"_id" : ObjectId("625010bb7d8490d5270b4424"),
	"name" : "FFF",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-15",
	"problem_solved" : 67
},

/* 3 createdAt:4/8/2022, 4:08:32 PM*/
{
	"_id" : ObjectId("625010a87d8490d5270b4423"),
	"name" : "EEE",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-10",
	"problem_solved" : 0
},

/* 4 createdAt:4/8/2022, 4:08:04 PM*/
{
	"_id" : ObjectId("6250108c7d8490d5270b4422"),
	"name" : "DDD",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-18",
	"problem_solved" : 24
},

/* 5 createdAt:4/8/2022, 4:07:44 PM*/
{
	"_id" : ObjectId("625010787d8490d5270b4421"),
	"name" : "CCC",
	"placement_attendence" : "A",
	"task_submission" : "2020-11-03",
	"problem_solved" : 0
},

/* 6 createdAt:4/8/2022, 4:06:48 PM*/
{
	"_id" : ObjectId("625010407d8490d5270b4420"),
	"name" : "BBB",
	"placement_attendence" : "A",
	"task_submission" : "2020-10-03",
	"problem_solved" : 81
},

/* 7 createdAt:4/8/2022, 4:06:26 PM*/
{
	"_id" : ObjectId("6250102a7d8490d5270b441f"),
	"name" : "AAA",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-30",
	"problem_solved" : 18
}	Query:

db.students.find({placement_attendence:"P"});
 


Output:

/* 1 createdAt:4/8/2022, 4:09:05 PM*/
{
	"_id" : ObjectId("625010c97d8490d5270b4425"),
	"name" : "GGG",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-31",
	"problem_solved" : 12
},

/* 2 createdAt:4/8/2022, 4:08:51 PM*/
{
	"_id" : ObjectId("625010bb7d8490d5270b4424"),
	"name" : "FFF",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-15",
	"problem_solved" : 67
},

/* 3 createdAt:4/8/2022, 4:08:32 PM*/
{
	"_id" : ObjectId("625010a87d8490d5270b4423"),
	"name" : "EEE",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-10",
	"problem_solved" : 0
},

/* 4 createdAt:4/8/2022, 4:06:26 PM*/
{
	"_id" : ObjectId("6250102a7d8490d5270b441f"),
	"name" : "AAA",
	"placement_attendence" : "P",
	"task_submission" : "2020-10-30",
	"problem_solved" : 18
}







