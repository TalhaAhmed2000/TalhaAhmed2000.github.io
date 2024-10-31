---
permalink: /markdown/
title: "Self-Learning Journey"
time_period: 
author_profile: true
redirect_from: 
  - /md/
  - /markdown.html
---


In the ever-evolving field of data science, continuous learning is not just an option but a necessity. The rapid pace at which this field is growing demands a commitment to self-improvement and the acquisition of new knowledge and skills. My journey into data science, a significant shift from my original focus in econometrics and mathematics, was accompanied by an even greater need for self-learning.

I owe a debt of gratitude to my esteemed professors, Dr. Ihsan Ayub Qazi, Dr. Muhammad Tahir, and Dr. Hassan Mohy-ud-Din. Their unwavering support and guidance not only kept me motivated but also taught me the value of appreciating the learning process, rather than solely fixating on the end results.

This section is dedicated to recounting my never-ending learning journey. I am committed to facing challenges head-on, exploring peer-reviewed journals, implementing newfound knowledge wherever possible, and, most importantly, embracing a spirit of perpetual learning.

### Recount 1: Value set iteration for two-person zero-sum Markov games

**Citation:** [Chang, Hyeong Soo. "Value set iteration for two-person zero-sum Markov games." Automatica 76 (2017): 61-64.](https://www.sciencedirect.com/science/article/pii/S0005109816304022?casa_token=AQJCvVqQsFoAAAAA:WEBXNexF9BlhIvp_V1PyXC6byIco-Cw_FhZK1qyvCpWvOO33KEbMIoaJOdjDkjTuHolV9IoxKWU)

#### Overview:
- The author ingeniously uses the concepts of policy/value set iteration i.e. generalized versions of policy and value iteration respecitvely to pose the standard bellman optimality algorithm as a *exact* mini-max game.
- Furthemore, the author shows great understanding of contraction mappings and using it to prove that the value set iteration algorithm shows atleast linear convergence for standard MG's unlike some variants of VI which require expnonential/polynomial convergence.
- Moreover, the author also shows that by optimally choosing a set of policies at the begining of each iteration (denoted as Policy Switching - PS), VSI can potentially improve the convergence speed in terms of the number of iterations.

#### Key Takeaways:
- Before reading this paper, I had only come across *exact* terminology when studying gradient descent and its various learning step methodologies including backtracking line search, inexact line search and **exact** line search. 
- It seemed quiti intuitive and simple at first, i.e. trying to find the optimal learning step by minimizing over all possiblities and choosing the one giving the lowest function value. But one swiftly realizes that solving this optimization problem is not practical for large scale systems.
- Here similarly in this picture, exact value set iteration i.e. choosing optimal *Expected Future Discounted Reward/Cost* at each iteration does seem to work quite well.  
- However, I believe its precisely due to the exact approach the author expresses that the algorithm is vulnerable to the curse of dimensionality and for large state/action spaces, the VSI algorithm becomes intractable. 

#### Notes/Thoughts/Future Direction:
- Currently working on implementing VSI and VSI - PS on 2D 3x3/4x4 Tic Tac Toe.
- Also thinking of extending it to 3D Tic Tac Toe but that may require some Deep Neural Networks to come into play to overcome the issue of curse of dimensionality.

### Recount 2: Paper Title - On Supervised Classification of Feature Vectors with Independent and Non-Identically Distributed Elements

**Citation:** [Shahrivari, Farzad, and Nikola Zlatanov. "On Supervised Classification of Feature Vectors with Independent and Non-Identically Distributed Elements." Entropy 23.8 (2021): 1045.](https://www.mdpi.com/1099-4300/23/8/1045)

#### Overview:
- The author proposes the *Nearest Empirical Distribution* Algorithm for supervised classification problems where the feature vectors are independent but not identically distributed (denoted by i.n.i.d).
- The author claims no novelty regarding the algorithm itself but, most importantly, in proving the following two key points:
  - Deriving an upper bound on the error probability (denoted by $\mathcal{P}_{e} = \operatorname{Pr}(X \neq \hat{X})$), which implies better interpretability and explainability—two key aspects to pursue in any machine learning model.
  - Showing that there exists at least one classifier with an asymptotically optimal error probability when at least one training feature vector per label is available, provided the length of the feature vector $n$ is large, i.e., $\mathcal{P}_{e} \stackrel{n}{\rightarrow} 0$.


#### Key Takeaways:
- What I found most interesting was the fact that even with as less as 1 training example per label, the classifier is asymtomatically optimal thereby reducing the effect of curse of dimensionality unlike some other algorithms like KNN or Naive Bayes, where as $n$ increases, the error probability increases. This does seem to imply that the algorithm can theoretically and practically outperform Deep Neural Networks (DNN) as they are data hungry.
- Furthermore, there exists a class of algorithms, known as *Independant Component Analysis*({ICA}) which can transform dependant, non-identitcally distributed feature vectors into i.-non.i.d.

#### Notes/Thoughts/Future Direction:
- Maybe a good idea to start looking into ICA algorithms since that seems to be the starting point when dealing with d.non.i.d which is most often come across in practice.
- One question comes to mind when the author assumed that the distribution of the feature vector with one label is not a *pertubation* of the distribution of the feature vector with another label. At first, one may conclude that having this assumption violated would negate the i-non.i.d assumption which is critical to the algorithm proposed. But why then we have to assume this is the case and not use the aforementioned ICA algorithm to make it i-non.i.d? Clarity may come when I read more into ICA and perhaps its limitations?
- The algorithm definetly seems quite straightforward to implement seeing as they nicely explained the steps for replicating the process one by one. 

### Recount 3: Paper Title - Work In Progress

**Citation:** [Author(s). "Paper Title." *Journal Name*, Year, Volume, Pages, DOI](Link to paper)

#### Overview:
- Provide an overview of the paper's subject matter and its significance.
- Explain the research methodology used in the paper.

#### Key Takeaways:
- Share your thoughts on what you found most remarkable or novel in the paper.
- Mention any gaps or questions that you believe should be explored in the future.

#### Notes/Implementation:
- Reference your personal notes or any practical implementations related to this paper.
- Include links to any code or documentation you've created during your study.



<!-- ## Locations of key files/directories

* Basic config options: _config.yml
* Top navigation bar config: _data/navigation.yml
* Single pages: _pages/
* Collections of pages are .md or .html files in:
  * _publications/
  * _portfolio/
  * _posts/
  * _teaching/
  * _talks/
* Footer: _includes/footer.html
* Static files (like PDFs): /files/
* Profile image (can set in _config.yml): images/profile.png

## Tips and hints

* Name a file ".md" to have it render in markdown, name it ".html" to render in HTML.
* Go to the [commit list](https://github.com/academicpages/academicpages.github.io/commits/master) (on your repo) to find the last version Github built with Jekyll. 
  * Green check: successful build
  * Orange circle: building
  * Red X: error
  * No icon: not built

## Resources
 * [Liquid syntax guide](https://shopify.github.io/liquid/tags/control-flow/)

## Markdown guide

### Header three

#### Header four

##### Header five

###### Header six

## Blockquotes

Single line blockquote:

> Quotes are cool.

## Tables

### Table 1

| Entry            | Item   |                                                              |
| --------         | ------ | ------------------------------------------------------------ |
| [John Doe](#)    | 2016   | Description of the item in the list                          |
| [Jane Doe](#)    | 2019   | Description of the item in the list                          |
| [Doe Doe](#)     | 2022   | Description of the item in the list                          |

### Table 2

| Header1 | Header2 | Header3 |
|:--------|:-------:|--------:|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|-----------------------------|
| cell1   | cell2   | cell3   |
| cell4   | cell5   | cell6   |
|=============================|
| Foot1   | Foot2   | Foot3   |

## Definition Lists

Definition List Title
:   Definition list division.

Startup
:   A startup company or startup is a company or temporary organization designed to search for a repeatable and scalable business model.

#dowork
:   Coined by Rob Dyrdek and his personal body guard Christopher "Big Black" Boykins, "Do Work" works as a self motivator, to motivating your friends.

Do It Live
:   I'll let Bill O'Reilly [explain](https://www.youtube.com/watch?v=O_HyZ5aW76c "We'll Do It Live") this one.

## Unordered Lists (Nested)

  * List item one 
      * List item one 
          * List item one
          * List item two
          * List item three
          * List item four
      * List item two
      * List item three
      * List item four
  * List item two
  * List item three
  * List item four

## Ordered List (Nested)

  1. List item one 
      1. List item one 
          1. List item one
          2. List item two
          3. List item three
          4. List item four
      2. List item two
      3. List item three
      4. List item four
  2. List item two
  3. List item three
  4. List item four

## Buttons

Make any link standout more when applying the `.btn` class.

## Notices

**Watch out!** You can also add notices by appending `{: .notice}` to a paragraph.
{: .notice}

## HTML Tags

### Address Tag

<address>
  1 Infinite Loop<br /> Cupertino, CA 95014<br /> United States
</address>

### Anchor Tag (aka. Link)

This is an example of a [link](http://github.com "Github").

### Abbreviation Tag

The abbreviation CSS stands for "Cascading Style Sheets".

*[CSS]: Cascading Style Sheets

### Cite Tag

"Code is poetry." ---<cite>Automattic</cite>

### Code Tag

You will learn later on in these tests that `word-wrap: break-word;` will be your best friend.

### Strike Tag

This tag will let you <strike>strikeout text</strike>.

### Emphasize Tag

The emphasize tag should _italicize_ text.

### Insert Tag

This tag should denote <ins>inserted</ins> text.

### Keyboard Tag

This scarcely known tag emulates <kbd>keyboard text</kbd>, which is usually styled like the `<code>` tag.

### Preformatted Tag

This tag styles large blocks of code.

<pre>
.post-title {
  margin: 0 0 5px;
  font-weight: bold;
  font-size: 38px;
  line-height: 1.2;
  and here's a line of some really, really, really, really long text, just to see how the PRE tag handles it and to find out how it overflows;
}
</pre>

### Quote Tag

<q>Developers, developers, developers&#8230;</q> &#8211;Steve Ballmer

### Strong Tag

This tag shows **bold text**.

### Subscript Tag

Getting our science styling on with H<sub>2</sub>O, which should push the "2" down.

### Superscript Tag

Still sticking with science and Isaac Newton's E = MC<sup>2</sup>, which should lift the 2 up.

### Variable Tag

This allows you to denote <var>variables</var>. -->
