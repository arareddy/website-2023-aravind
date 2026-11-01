---
# Leave the homepage title empty to use the site title
title: 
date: 2025-11-11
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: markdown
    id: news
    content:
      title: News
      text: |-
        - **Oct 2026:** Our US$100,000 Google Research Gift project on multilingual AI safety evaluation for agents began. I lead the effort at CeRAI.
        - **Oct 2026:** [X-AVDD](/publication/x-avdd/), on audio-visual dataset distillation, was accepted at NeurIPS 2026 and is now on arXiv.
        - **Oct 2026:** New preprint on [machine unlearning for federated socially fair k-means](/publication/machine-unlearning-federated-kmeans/).
        - **Jul 2026:** Released [Pluralis v0.1](/publication/pluralis/), a multicultural, multimodal, multilingual benchmark for AI risk and reliability.
        - **Mar 2026:** [DiRe](/publication/dire/), on dataset condensation, appeared at WACV 2026.
        - **Nov 2025:** Joined the Centre for Responsible AI at IIT Madras as a Principal Project Scientist.
        - **Apr 2025:** Granted [US Patent 12,288,237](/publication/nonsymmetric-dpp-patent/) on online inference for nonsymmetric DPPs.
    design:
      columns: '2'
  - block: markdown
    id: research
    content:
      title: Research
      text: |-
        My research is in **Theoretical Machine Learning**, grounded in theoretical computer science, and extends into **Responsible AI** and **Computer Vision**. Theory is the foundation: my work in the other two areas builds on it.

        ### Theoretical Machine Learning

        I design algorithms with provable guarantees, often going beyond worst-case analysis to explain why algorithms work on real data even when their worst-case bounds are pessimistic. My three best papers are from this line of work:

        - [One-pass MAP inference for nonsymmetric DPPs](/publication/one-pass-nonsymmetric-dpp/) (ICML 2022), which started the study of streaming and online MAP inference for these models. I am the sole first and corresponding author, and the work led to a granted US patent.
        - [LP recovery guarantees for MAP inference](/publication/beyond-perturbation-stability/) (AISTATS 2021), which gives a new explanation of why a standard LP relaxation succeeds on real vision instances. I am co-first author.
        - [Improved guarantees for k-means++ and its parallel variant](/publication/kmeans-plus-plus/) (NeurIPS 2020), which improves the k-means++ bound from 8(ln k + 2) to 5(ln k + 2) for an algorithm that is the default in widely used libraries.

        I have also worked on dynamic and adaptive algorithms for [tensor product regression](/publication/dynamic-tensor-product-regression/) (NeurIPS 2022), [pairwise summation](/publication/adaptive-dynamic-hashing/) (IEEE BigData 2022) and [Mahalanobis distance estimation](/publication/online-adaptive-mahalanobis/) (IEEE BigData 2023).

        ### Responsible AI

        I use these tools to ask when an AI system can be trusted: whether it is fair, whether it can forget data on request, and whether it is safe in the cultural contexts where it is used.

        - With Dr. Sunayana Sitaram, I am India lead of [Pluralis](/publication/pluralis/), a culture-first multimodal safety benchmark that is part of the MLCommons AILuminate effort, with 6,448 image-text prompts across six Asia-Pacific locales and eight languages. CeRAI led benchmark design, curation and validation for English, Hindi and Tamil.
        - Under a Google Research Gift, I lead CeRAI's effort on multilingual, multicultural evaluation of AI agents.
        - With Prof. Saurav Prakash, I work on [fair, deletable clustering](/publication/machine-unlearning-federated-kmeans/). We prove an O(log² k) guarantee for federated socially fair k-means that does not depend on how groups are split across institutions, using our NeurIPS 2020 bound as a black box, and we show that replay reproduces retraining exactly.

        ### Computer Vision

        Training vision models for genomics at the Broad Institute took months of compute, which led me to dataset distillation: synthesizing a small dataset with nearly the training value of a large one. With Dr. Konda Reddy Mopuri and Saumyaranjan Mohanty, I developed [DiRe](/publication/dire/) (WACV 2026), a diversity regularizer that draws on my work on diverse subsets and improves eight leading methods from CIFAR-10 to ImageNet-1K, and [X-AVDD](/publication/x-avdd/) (NeurIPS 2026), which brings distillation to audio-visual data, cutting synthesis time from 10 to 1.3 GPU-hours and roughly tripling accuracy on VGGSound.

        ### Research plan

        In the next two to three years, I want to build a group of PhD and MS students, funded initially by the Google gift (until March 2028), around three directions that apply theory to open problems from my recent work:

        1. **Fair and frugal multilingual evaluation:** compressing AI safety benchmarks into small representative subsets while minimizing the worst error across languages, so that low-resource languages are not sacrificed for accuracy on English.
        2. **Diversity-aware benchmark creation:** treating benchmark construction as online diverse-subset selection, so that each new item is accepted only if it adds coverage.
        3. **Diversity with guarantees for data-efficient vision:** replacing heuristic diversity penalties with principled objectives, and proving when a distilled dataset preserves the training signal of the full data.

        In the longer term, I aim for a theory of how little data, how few evaluations and how cheap an update an AI system needs while remaining fair and safe.
    design:
      columns: '2'
  - block: collection
    id: publications
    content:
      title: Publications
      text: |-
        Eight peer-reviewed conference papers: four at CORE A\* venues and two at CORE A venues, under the [ICORE2026 Conference Ranking](https://portal.core.edu.au/conf-ranks/). Seven are published and one is accepted at NeurIPS 2026. [DiRe](/publication/dire/) and [X-AVDD](/publication/x-avdd/) are post-Ph.D. work.
      count: 0
      filters:
        folders:
          - publication
        publication_type: '1'
    design:
      view: citation
      columns: '2'
  - block: collection
    content:
      title: Preprints
      count: 0
      filters:
        folders:
          - publication
        publication_type: '3'
    design:
      view: citation
      columns: '2'
  - block: collection
    content:
      title: Patents
      count: 0
      filters:
        folders:
          - publication
        publication_type: '8'
    design:
      view: citation
      columns: '2'
  - block: markdown
    id: funding
    content:
      title: Funding and Awards
      text: |-
        ### Research funding

        **Google Research Gift, US$100,000** (Oct 2026 to Mar 2028)<br>
        *Scaling Pluralis to Enable Multilingual AI Safety Evaluation for Agents Across the Globe.*<br>
        Co-authored the proposal with Dr. Lora Aroyo (Google DeepMind); project lead at CeRAI. PI: Prof. Balaraman Ravindran, IIT Madras.

        **Adobe Research Gift, US$20,000** (2022)<br>
        *Dimension Reduction to Enable Learning on the Edge.*<br>
        Co-authored the proposal with Dr. Zhao Song and Dr. Ritwik Sinha (Adobe Research). PI: Prof. Aravindan Vijayaraghavan, Northwestern University.

        ### Selected awards

        - Silver Reviewer Award, ICML 2026 Position Paper Track (2026)
        - NeurIPS Scholar Award, US$2,000 (2022)
        - Peter and Adrienne Barris Outstanding TA Award, Northwestern University ([press release](https://www.mccormick.northwestern.edu/computer-science/news-events/news/articles/2022/northwestern-cs-announces-spring-2022-outstanding-teaching-assistant-and-peer-mentors.html)) (2022)
        - CS Supplemental Award, US$3,000, Northwestern University, for top CS Ph.D. applicants (2018)
        - Charpak Scholarship for Research Internship, Government of France (2017)
        - All India Rank 189, JEE Advanced (2014)
        - Gold Medallist, Indian National Physics Olympiad (2014)
    design:
      columns: '2'
  - block: markdown
    id: teaching
    content:
      title: Teaching
      text: |-
        I taught four courses as a Visiting Assistant Professor at IIT Hyderabad and have given guest lectures in Machine Learning I at IIT Madras.

        ### Instructor, IIT Hyderabad

        | Course | Term | Enrolled | Instructor / course rating |
        |---|---|---|---|
        | Convex Optimization / Optimization-I (AI 2101 / AI 1233), 3 credits, UG | Jan to May 2025 | 158 | 4.02 / 4.03 |
        | Programming for AI (AI 1013), 2 credits, co-taught with Dr. P. N. Karthik | Jan to Apr 2025 | 36 | 4.58 / 4.71 |
        | Introduction to Modern Artificial Intelligence (AI 1001), 1 credit, UG | Sep to Oct 2024 | 103 | 4.02 / 4.07 |
        | Introduction to Submodular Functions (EE 5328), 1 credit, PG | Jul to Sep 2024 | 5 | 4.70 / 4.35 |

        Ratings are out of 5.

        ### Teaching interests

        I prefer courses of a mathematical nature related to machine learning and algorithms, and I can teach core courses in both CSE and Data Science and AI, such as Data Structures and Algorithms, Discrete Mathematics, Machine Learning, Optimization, and Probability and Statistics. I would also like to develop two new courses:

        - **Beyond Worst-Case Analysis**, with a focus on topics such as clustering, robust statistics, topic models and algorithms with predictions.
        - **Submodular Optimization and Applications to Machine Learning**, a full 3-credit extension of the course I taught at IIT Hyderabad.

        ### Guest lectures

        - Maximum Likelihood and Probabilistic Linear Regression, Machine Learning I, IIT Madras (Aug 2026; one week, three lectures)
        - Submodular Function Maximization, Algorithms for Big Data, Northwestern University (Apr 2022)
        - Introduction to Markov Chains, Math Toolkit for TCS, Northwestern University (May 2019)

        ### Teaching assistant

        - Mathematical Foundations of Computer Science (CS 212), Northwestern University: Spring 2022, Fall 2020, Fall 2019. Received the Peter and Adrienne Barris Outstanding TA Award for Spring 2022.
        - Design and Analysis of Algorithms (CS 336), Northwestern University: Winter 2019
        - Fundamentals of Computing (ESC 101), IIT Kanpur: Winter 2018
    design:
      columns: '2'
  - block: markdown
    id: mentoring
    content:
      title: Mentoring
      text: |-
        ### Project mentor, WSAI Summer Internship Program, IIT Madras

        Faculty guide: Prof. B. Ravindran.

        - Madhangi Karimanal, B.E. (CSE), SSN College of Engineering (May to Jul 2026). Co-author of Pluralis v0.1.
        - Paruchuri Sriram, M.Tech. (CSE), IIIT Hyderabad (May to Jul 2026). Project: *Saakshya: A Multi-Agent, RAG-Enhanced Framework for Deepfake Detection and Governance.*

        ### Informal research mentoring

        - Saumyaranjan Mohanty, Ph.D. student, IIT Hyderabad (advisor: Dr. Konda Reddy Mopuri). Joint papers: DiRe (WACV 2026) and X-AVDD (NeurIPS 2026).
        - Mohd Wasif Raza, M.S. student (EE), IIT Madras. Co-first author on machine unlearning for federated socially fair k-means.
        - Deeraj S K, B.Tech. student, SVNIT Surat, and WSAI summer intern (faculty guide: Dr. Saurav Prakash). Co-first author on the same paper.
        - Akanksha Singh, Post-baccalaureate Fellow, WSAI, IIT Madras (faculty guide: Prof. B. Ravindran).
        - Vraj Thakkar, Post-baccalaureate Fellow, WSAI, IIT Madras (faculty guide: Dr. Krishna Pillutla).
    design:
      columns: '2'
  - block: markdown
    id: talks
    content:
      title: Talks and Service
      text: |-
        ### Invited research talks

        - *On MAP Inference of Ferromagnetic Potts Models and Nonsymmetric DPPs:* IIT Madras, Department of Data Science and AI (Sep 2024), IIT Kanpur, Department of CSE (Jun 2024), IISc Bangalore ([recording](https://youtu.be/KvncwqMKKgE)) (May 2024), IIT Hyderabad, Department of CSE (May 2024)
        - *On Clustering, MAP Inference, and Causal Inference:* Broad Institute of MIT and Harvard (Nov 2022), Stanford University (Oct 2022)
        - *Beyond Perturbation Stability:* University of Chicago Theory Lunch (Nov 2022)

        ### Service

        - **Conference reviewer:** AAAI (2026), AISTATS (2023 to 2024), ECCV (2026), FSTTCS (2024), ICLR (2022 to 2024), ICML (2022 to 2026), NeurIPS (2021 to 2025)
        - **Outreach:** Workshop Leader and Mentor, NeurIPS 2022 High-School Outreach Program; invited talks for school students at RSI-C Chennai (May 2026) and Oak Valley International School, Hyderabad (Jun 2025)
        - **Community:** Board Member, CS Ph.D. Advisory Council, Northwestern University (2020 to 2022); Webmaster, Northwestern CS Theory group (2018 to 2023)
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      email: aravind@cerai.in
      address:
        street: Room 670, New Academic Complex (NAC) 2 
        city: Indian Institute of Technology Madras
        region: Chennai, Tamil Nadu
        postcode: '600036'
        country: India
        country_code: IN
      # Automatically link email and phone or display as text?
      autolink: true
    design:
      columns: '2'
---
