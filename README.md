# motivation_reddit

This dataset contains comments collected from Reddit about motivational factors in physical activities. 
The format of the file is :
```
{
        "sample_id": 729,
        "id": "r/AskReddit/comments/t3_3h7kg3/comment/cu5com6/",
        "question": "r.AskMen.guys_who_work_out_regularly_how_do_you_motivate",
        "labels": [
            "physical appearance"
        ]
},
```
where, 

* id - is the identifier of the comment. The general structure is `"r/AskReddit/comments/{post_id}/comment/{comment_id}/"`

* question - is the post id the comment addressed

* labels - list of one or more factors that are associated with this comment, out of 10 options ["physical appearance", "physical health", "mental health", "habit formation", "socializing and group training", "enjoyable activities", "set goals", "media use", "app monitoring", "financial commitment"]

To get the content of the comments content you will need to use the [Reddit openshift API](https://github.com/pushshift/api) and use the `id` to fetch the context.

For example, for this id `"r/AskReddit/comments/t3_3h7kg3/comment/cu5com6/"`, the content is:

`"I have goals to make a high level rugby side and i need to be fit and strong to get there."`

If you are using this dataset please cite this work: TBD
