# hackathon-6-challenge

In this challenge you will have to predict whether a person will become un-employed in the next 12 months.

It is a binary classification task.

You will be given the training set as follows:

```
~ > head train.csv

id,birth date,job type,school level,domestic status,profession,domestic relationship type,ethnicity,gender,earned dividends,interest earned,monthly work,country of origin,target
15463,1983-12-26,private,secondary,single,mechanic,never married,afro american,Female,0,0,160,u.s.,1
2202,1962-12-31,private,college graduate,spouse passed,secretarial,never married,white and privileged,Female,0,0,160,u.s.,1
29145,1979-12-27,private,college graduate,married 2,C-level,has husband,white and privileged,Female,0,0,200,u.s.,0
11330,1965-12-30,private,entry level college,married 2,sales,has husband,white and privileged,Female,0,0,208,canada,0
20822,1967-12-30,self-emp-inc,entry level college,divorce pending,C-level,never married,white and privileged,Female,0,0,300,u.s.,1
12218,1996-12-22,unknown,entry level college,single,unknown,living with child,white and privileged,Female,0,0,140,u.s.,1
17810,1974-12-28,private,secondary-5 through 6,d,estate employee,never married,white and privileged,Female,0,0,160,mexico,1
14036,1981-12-26,local-gov,secondary,married 2,secretarial,has husband,white and privileged,Female,0,0,160,u.s.,0
13802,1993-12-23,private,10th,d,household labor,never married,white and privileged,Female,0,0,232,u.s.,1
```

Where `target` is the target column.

## Submission and evaluation

### Providing predictions

You will be expected to deploy a server [on heroku](https://github.com/LDSSA/heroku-example) in which observations will
arrive over a period of a few weeks and the predictions you return will be used in the grading.

Please refer to the [calendar](https://calendar.google.com/calendar/b/2?cid=bGlzYm9uZGF0YXNjaWVuY2Uub3JnX2pjaWYwZnJyMzk3YXBoZzB0cGhuN2w2N2FnQGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20), [hackathon description document](https://docs.google.com/document/d/1AqZ8JPzkaBkEeeESJHhkyVrw9sr2DYg_tldfJLutVeY/edit?usp=sharing), and [report specification](https://docs.google.com/document/d/1mmbOgLub_UaP_dckjwuhwz8ExurDpJaTz_D6woBEfE8/edit?usp=sharing) for details on the hackathon.

### Evaluation

Your model will be evaluated on it's ranking ability ([ROC_AUC_SCORE](http://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html))

Like the other hackathons you will be evaluated in two main components:

- The ranking ability of your model
- The approach you take and how well you communicate it

The scoring is not finalized yet but you can be sure that you will not be able to win the hackathon only with a good model.
You will also need to do an excellent job on the reporting as well.
