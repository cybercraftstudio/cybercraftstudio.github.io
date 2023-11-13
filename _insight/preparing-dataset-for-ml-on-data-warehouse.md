---
title: "Preparing Your Dataset for Machine Learning on Data Warehouse"
description: "Preparing your dataset for machine learning on data warehouse feels like an impossible task, but it doesn’t have to be. Here are expert insights on how to get it right from the start!"
post_img: "/images/uploads/sites/5/2022/10/news-cover-2.jpeg"
post_detail: "Data preparation for machine learning is non-negotiable, especially in today’s world where virtually all business operations are data-driven. According to a recent IDC market..."
post_reading_time: 7
category: "Article"
show_lets_meet_section: true
weight: 12
related_insights:
  [
    "/insight/data-engineering-concepts-approaches/",
    "/insight/serverless-architecture/",
  ]
meta_img: "/images/uploads/sites/5/2022/10/news-cover-2.jpeg"
meta_image_width: 857
meta_image_height: 570
meta_type: "article"
meta_updated_time: "2023-03-03T10:48+00:00"
meta_published_time: "2022-10-05T10:07+00:00"
meta_modified_time: "2023-03-03T10:48+00:00"
meta_card: "summary_large_image"
---
<section class="post-body pb-3 pb-md-5">
  <div class="container">
    <div class="row justify-content-md-center justify-content-lg-start">
      <div class="col-lg-9 col-xl-8 mb-3 mb-md-0">
        <h1 class="txt-ttl-2 cl-black mb-4">
          {{ page.title }}
        </h1>
        <div class="row mb-5 d-none">
          <div class="col-4">
            <div class="b-quote">
              <h4 class="txt-ttl-4 cl-black mb-3">Categories</h4>
              <ul class="list-reset">
                <li>{{ page.category }}</li>
              </ul>
            </div>
          </div>
        </div>
        <nav class="side-nav mod-mob mb-3 py-4 d-lg-none">
          <div class="ss-pad">
            <div class="txt-ttl-5 cl-black mb-3">
              Table of content
            </div>
            <nav id="content-table" class="side-nav mod-simple">
              <ul class="nav nav-pills list-reset">
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#data-preparation-for-machine-learning"
                    >What is Data Preparation for Machine Learning?</a
                  >
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#machine-learning-definition-goals-types"
                    >Machine Learning Definition, Goals, and Types</a
                  >
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#data-preparation-for-machine-learning-best-practices"
                    >How to Prepare Data for Machine Learning - Best
                    Practices</a
                  >
                </li>
                <li class="nav-item">
                  <a target="_self" class="nav-link" href="#sum-up">Sum Up</a>
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#faq-dataset-for-ml-on-data-warehouse"
                    >FAQs on Dataset for Machine Learning on Data Warehouse</a
                  >
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#cross-industry-standard-process-for-data-mining"
                    >Cross Industry Standard Process for Data Mining
                    (CRISP-DM)</a
                  >
                </li>
              </ul>
            </nav>
          </div>
        </nav>
        <article class="editor-content has-toc mb-3 mb-lg-5">
          <p>
            Data preparation for machine learning is non-negotiable, especially
            in today’s world where virtually all business operations are
            data-driven. According to a recent IDC market research report, the
            volume of data collected in the
            <a
              href="https://www.forbes.com/sites/forbestechcouncil/2021/10/14/flying-blind-how-bad-data-undermines-business/?sh=2d24438f29e8"
              data-type="URL"
              data-id="https://www.forbes.com/sites/forbestechcouncil/2021/10/14/flying-blind-how-bad-data-undermines-business/?sh=2d24438f29e8"
              target="_blank"
              rel="noreferrer noopener"
              >next three years</a
            >
            will be more than what businesses collected in the last three
            decades!<br />With massive amounts of data generated today,
            maintaining data quality is no easy task. However, it doesn’t have
            to be. In this eye-opening guide, we will walk you through how to
            prepare data for machine learning, as early as now before your data
            sets become overwhelming. Read on!
          </p>
          <h3 id="data-preparation-for-machine-learning">
            What is Data Preparation for Machine Learning?
          </h3>
          <p>
            Data preparation or data pre-processing is the process of gathering
            and combining raw data before structuring and organizing it for
            business analysts to run it through machine learning algorithms.
            Data preparation is the most basic step when a business is trying to
            solve real-world challenges faced by consumers through
            <a
              href="/insight/data-engineering-best-practices/"
              data-type="URL"
              data-id="data-engineering-best-practices.html"
              >data engineering</a
            >
            and machine learning applications.
          </p
          <figure class="wp-block-image size-large">
            <img
              width="1024"
              height="892"
              src="/images/uploads/sites/5/2022/10/1726-1-1024x892.png"
              alt=""
              class="wp-image-25895"
              srcset="
                /images/uploads/sites/5/2022/10/1726-1-1024x892.png 1024w,
                /images/uploads/sites/5/2022/10/1726-1-300x261.png   300w,
                /images/uploads/sites/5/2022/10/1726-1-768x669.png   768w,
                /images/uploads/sites/5/2022/10/1726-1.png          1918w
              "
              sizes="(max-width: 1024px) 100vw, 1024px"
            />
          </figure>
          <p><br />Preparing data for machine learning is important because:</p>
          <p>
            <strong>ML Algorithms Work with Numbers</strong><br />A typical data
            set is usually presented in numerous tables featuring rows and
            columns, although every type of data might have different variables.
            For instance, some data types may have numeric variables, such as
            integers, percentages, rates, or even ranks. Other prevalent
            variables used in data presentation include names and categories, or
            binary options such as true or false.
          </p>
          <p>
            However, machine learning algorithms only work with numeric data.
            Technically, these algorithms take numerical inputs and give
            predictions (output) in numbers. That’s why data scientists usually
            view ML data as vectors and matrices.
          </p>
          <p>
            <strong
              >Businesses Must Meet the Requirements of ML Algorithms<br /></strong
            >Businesses have a plethora of options when it comes to choosing a
            machine learning algorithm, depending on the foregoing predictive
            modeling project. That said, these algorithms have distinct
            requirements, as well as expectations when it comes to data input.
          </p>
          <p>
            For instance, an algorithm, such as a linear machine model might
            require a specific probability distribution (Gaussian) for each
            input and target variable. In that case, machine learning data
            preparation will help change the input variables to match Gaussian
            probability distribution, or change the ML algorithm altogether to
            reconfigure data input expectations.
          </p>
          <h3 id="machine-learning-definition-goals-types">
            Machine Learning Definition, Goals, and Types
          </h3>
          <p>
            Machine learning, popularly abbreviated as ML is a special
            artificial intelligence (AI) tech that empowers software
            applications to give nearly accurate predictive outcomes, without
            necessarily programming them. The goal of this tech is to optimize
            computer systems to become smarter and more intelligent with little
            to zero human interference. Typically, this entails building
            programs that can handle specific practical learning tasks. Another
            goal for ML is to come up with elaborate computations of human
            learning processes and perform programmed simulations based on them.
          </p>
          <figure class="wp-block-image size-large">
            <img
              loading="lazy"
              width="1024"
              height="337"
              src="/images/uploads/sites/5/2022/10/5-1-1024x337.png"
              alt=""
              class="wp-image-25897"
              srcset="
                /images/uploads/sites/5/2022/10/5-1-1024x337.png 1024w,
                /images/uploads/sites/5/2022/10/5-1-300x99.png    300w,
                /images/uploads/sites/5/2022/10/5-1-768x253.png   768w,
                /images/uploads/sites/5/2022/10/5-1.png          1918w
              "
              sizes="(max-width: 1024px) 100vw, 1024px"
            />
          </figure>
          <p>There are three types of machine learning, including:</p>
          <h5>Supervised Learning</h5>
          <p>
            According to Gartner, supervised learning will probably be the most
            prevalent machine learning among enterprise IT leaders throughout
            2022 and beyond. As the name suggests, the machine is supervised
            while learning as the data scientists feed in the algorithm
            information.
          </p>

          <p>
            Supervised learning works by feeding pairs of historical input and
            output data to ML algorithms, which creates an output that is nearly
            as accurate as the desired outcome. Prevalent algorithms used in
            supervised learning ML include neural networks and linear
            regression.
          </p>

          <p>
            This type of ML is used in various real-world use cases, such as:
          </p>

          <ul>
            <li>
              <span style="color: initial;"
                >Determination of low-risk and high-risk loan applicants</span
              >
            </li>
            <li>Prediction of future real estate prices</li>
            <li>Determination of disease risk factors</li>
            <li>Prediction of failures in a system’s mechanical parts</li>
            <li>Revealing fraudulent bank transactions</li>
          </ul>

          <h5>Unsupervised Learning</h5>

          <p>
            Unsupervised learning is common in ML applications that seek to
            identify various data patterns in a set and draw conclusive insights
            from them. Unlike supervised learning, this ML doesn&#8217;t require
            constant human intervention to learn. Instead, it automatically
            detects less obvious patterns in a data set using a host of
            algorithms, such as Hidden Markov models, hierarchical clustering,
            or even k-means.
          </p>

          <p>
            Unsupervised learning ML is instrumental in creating predictive
            models. Examples of its uses cases in real-world scenarios include:
          </p>

          <ul>
            <li>
              Inventory clustering based on manufacturing or sales metrics
            </li>
            <li>Customer grouping based on purchase history and trends</li>
            <li>Segmenting correlations in customer data</li>
          </ul>

          <h5>Reinforced Learning</h5>

          <p>
            Reinforced learning is probably the closest ML that mimics how
            humans learn. Typically, the leveraged algorithm learns through
            direct interactions with the environment in question, to give a
            positive or negative reward. Prevalent algorithms used in reinforced
            learning include Q-learning, temporal difference, or even deep
            adversarial networks.
          </p>

          <p>
            However, reinforced learning isn&#8217;t a go-to ML application for
            many organizations because it requires enormous computation power to
            execute. But at the same time reinforced learning requires less
            human supervision, making it ideal when working on unlabeled data
            sets.
          </p>

          <p>
            Although real-world use cases for reinforced learning are still a
            work in progress, some examples include:
          </p>

          <ul>
            <li>Teaching cars to drive or park autonomously</li>
            <li>Dynamic traffic lights control to ease jam congestion</li>
            <li>
              Robotics training using raw video images for systems to simulate
              what they see
            </li>
          </ul>

          <h3 id="data-preparation-for-machine-learning-best-practices">
            How to Prepare Data for Machine Learning &#8211; Best Practices
          </h3>

          <p>
            Data preparation for machine learning can be an in-house DIY task or
            an
            <a
              href="/service/data-and-analytics/"
              data-type="URL"
              data-id="/service/data-and-analytics/"
              >outsourced data engineering service</a
            >, depending on the company policy and the amount of data that you
            are dealing with. Nonetheless, you can
            <a
              href="/insight/data-engineering-concepts-approaches/#etl-data-pipeline-steps"
              data-type="URL"
              data-id="data-engineering-concepts-approaches.html#etl-data-pipeline-steps"
              >prepare data</a
            >
            for machine learning in the following simple steps:
          </p>

          <p>
            <strong>Problem Formulation</strong><br />Which problem is your
            business trying to solve? Getting an answer to this question will
            not only help you prepare data the right way but also build a
            successful ML model by understanding what and how to do it.
          </p>

          <p>
            You can do this by going back to the basics, away from data. Spend
            quality time with the professionals within the domain in question to
            get a better understanding of the problems being solved. After that,
            use your findings to formulate a hypothesis of the factors and
            forces in play to determine which type of data you are going to
            capture or focus on. This will help you come up with a practical
            machine learning problem to be solved.
          </p>

          <p>
            <strong>Data Collection and Discovery</strong><br />Your data
            science team will proceed to collect and discover various data sets
            after establishing the real problem to be solved. This phase
            includes capturing various data sources from within the enterprise
            and third parties as well. An important factor, this process
            shouldn&#8217;t only focus on what the data ought to represent.
            Instead, it should also extend to reveal what the data might mean,
            especially when leveraged in different contexts. This is not to
            forget any factor that might have biased the data.
          </p>

          <p>
            Determining any bias, and its extent at data collection points will
            help mitigate biases in the ML in the long haul. Let’s assume you
            want to create a machine learning model that predicts consumer
            behavior. In that case, you can investigate bias by establishing
            whether the data was collected from diverse customer bases,
            perspectives, as well as geographical locations.
          </p>

          <p>
            <strong>Data Cleansing and Validation</strong><br />After
            investigating bias, it&#8217;s time to determine whether you have
            clean data that will give you the highest quality information to
            drive key decisions in your organization. Innovative data cleansing
            and validation tools, as well as techniques, can help you spot
            outliers, anomalies, inconsistencies, or even missing sets of data
            altogether. This will in turn help you to factor in missing values
            as neutrals or mitigate their impact on the final ML model.
          </p>

          <p>
            <strong>Raw Uncompressed Data Backup</strong><br />Raw uncompressed
            data is just as important as structured data since it might contain
            vital information about your brand. In that case, you would want to
            back it up before sorting and structuring. Moreover, raw data is the
            foundation of any downstream analysis when it comes to implementing
            machine learning models in your organization.
          </p>

          <p>
            Also, it&#8217;s worth noting that some variables in raw
            uncompressed data such as time points in interviews are unique and
            nigh impossible to reproduce. With this in mind, you&#8217;d want to
            back it up as well.
          </p>

          <p>
            <strong>Data Structuring</strong><br />Once you are satisfied with
            the type and volume of data, it will now help if you structure it
            before employing preferred ML algorithms. Typically any ML algorithm
            will work better and effectively if your data is structured into
            various categories, as opposed to simply uploading it in raw
            numbers. Prevalent effective practices, but often overlooked when
            preparing data for machine learning are data smoothing and binning
            continuous features.
          </p>

          <p>
            Smoothing as a continuous feature enhances denoising raw data by
            imposing casual assumptions in data extractions processes. This
            practice points out relationships in ordered data sets to give an
            easy-to-follow and understand order among data sets. Binning on the
            other hand structures data sets into bins using equi-statistical
            methods.
          </p>

          <p>
            Other practices for data structuring in preparation for ML
            application include:
          </p>

          <ul>
            <li>Data reduction</li>
            <li>Data normalization</li>
            <li>Data segmentation, based on training and testing ML models</li>
          </ul>

          <p>
            <strong>Feature Engineering and Selection</strong><br />This is the
            last stage in data preprocessing before delving deeper into building
            an effective machine learning model. Feature engineering entails
            creating or topping up new variables to enhance the ML model’s
            output. For instance, a data scientist may extract, aggregate, or
            even decompose various variables from a data set before transforming
            the features depending on probability distributions.
          </p>

          <p>
            Feature selection in this case entails pinpointing the relevant
            features to focus on and doing away with the non-essential ones.
            Inasmuch as a feature might look promising, it&#8217;s your
            responsibility to ensure that it doesn’t bring model training and
            over-lifting challenges when analyzing new data.
          </p>

          <h3 id="sum-up">Sum Up</h3>

          <p>
            Machine learning data preparation will help you build a successful
            ML model to drive key decisions in your organization. This guide
            explains the practices in a basic, layman&#8217;s language However,
            in the real sense, it takes an experienced data scientist or even a
            team of experts to do it effectively. That said, never hesitate to
            seek professional help when preparing data for machine learning.
            Contact us today and find out how our data experts can be of help.
          </p>

          <h3 id="faq-dataset-for-ml-on-data-warehouse">
            FAQs on Dataset for Machine Learning on Data Warehouse
          </h3>

          <section class="block-basic-accordion">
            <div
              class="block-basic-accordion-wrapper"
              id="accordion-group-block_62f64d9d75487"
            >
              <div class="basic-acc--item card">
                <a
                  class="basic-acc--item-head py-3 flex-align-center collapsed cl-inherit"
                  href="#accordion-item-block_62f64d9d75487-0"
                  data-toggle="collapse"
                  aria-expanded="false"
                >
                  <h3 class="txt-ttl-3 fw-700 flex-1 mb-0">
                    <span class="txt-ttl-4"
                      >How do you prepare a dataset for machine learning in
                      Python?</span
                    >
                  </h3>
                  <div class="rotating-icon-180 ml-auto">
                    <svg class="svg-icon">
                      <use xlink:href="#icon-arrow-down"></use>
                    </svg>
                  </div>
                </a>
                <div
                  data-parent="#accordion-group-block_62f64d9d75487"
                  id="accordion-item-block_62f64d9d75487-0"
                  class="collapse"
                >
                  <div class="editor-content pb-3">
                    <p>
                      You can leverage various libraries to prepare a dataset
                      for machine learning in Python, such as NumPy, pandas, and
                      sci-kit learn. The process is as follows:
                    </p>
                    <ul>
                      <li>Collect the data set</li>
                      <li>Handle any missing data</li>
                      <li>Encode categorical data</li>
                      <li>
                        Categorize the data into training and testing sets
                      </li>
                      <li>Perform feature engineering and selection</li>
                    </ul>
                  </div>
                </div>
              </div>
              <div class="basic-acc--item card">
                <a
                  class="basic-acc--item-head py-3 flex-align-center collapsed cl-inherit"
                  href="#accordion-item-block_62f64d9d75487-1"
                  data-toggle="collapse"
                  aria-expanded="false"
                >
                  <h3 class="txt-ttl-3 fw-700 flex-1 mb-0">
                    <span class="txt-ttl-4"
                      >Why is data preparation necessary in machine
                      learning?</span
                    >
                  </h3>
                  <div class="rotating-icon-180 ml-auto">
                    <svg class="svg-icon">
                      <use xlink:href="#icon-arrow-down"></use>
                    </svg>
                  </div>
                </a>
                <div
                  data-parent="#accordion-group-block_62f64d9d75487"
                  id="accordion-item-block_62f64d9d75487-1"
                  class="collapse"
                >
                  <div class="editor-content pb-3">
                    <p>
                      Data preparation for ML is important because machine
                      learning algorithms can only be effective when data is
                      formatted in a specific way.
                    </p>
                  </div>
                </div>
              </div>
              <div class="basic-acc--item card">
                <a
                  class="basic-acc--item-head py-3 flex-align-center collapsed cl-inherit"
                  href="#accordion-item-block_62f64d9d75487-2"
                  data-toggle="collapse"
                  aria-expanded="false"
                >
                  <h3 class="txt-ttl-3 fw-700 flex-1 mb-0">
                    <span class="txt-ttl-4"
                      >How do you prepare data for a model?</span
                    >
                  </h3>
                  <div class="rotating-icon-180 ml-auto">
                    <svg class="svg-icon">
                      <use xlink:href="#icon-arrow-down"></use>
                    </svg>
                  </div>
                </a>
                <div
                  data-parent="#accordion-group-block_62f64d9d75487"
                  id="accordion-item-block_62f64d9d75487-2"
                  class="collapse"
                >
                  <div class="editor-content pb-3">
                    <p>
                      You can prepare data for a model in the following steps:
                    </p>
                    <ul>
                      <li>Formulate problems to be solved</li>
                      <li>Collect data sets</li>
                      <li>Cleanse and validate data sets</li>
                      <li>Backup and structure the raw data</li>
                    </ul>
                  </div>
                </div>
              </div>
              <div class="basic-acc--item card">
                <a
                  class="basic-acc--item-head py-3 flex-align-center collapsed cl-inherit"
                  href="#accordion-item-block_62f64d9d75487-3"
                  data-toggle="collapse"
                  aria-expanded="false"
                >
                  <h3 class="txt-ttl-3 fw-700 flex-1 mb-0">
                    <span class="txt-ttl-4"
                      >What data do you use for machine learning?</span
                    >
                  </h3>
                  <div class="rotating-icon-180 ml-auto">
                    <svg class="svg-icon">
                      <use xlink:href="#icon-arrow-down"></use>
                    </svg>
                  </div>
                </a>
                <div
                  data-parent="#accordion-group-block_62f64d9d75487"
                  id="accordion-item-block_62f64d9d75487-3"
                  class="collapse"
                >
                  <div class="editor-content pb-3">
                    <p>
                      <span style="font-weight: 400;"
                        >The type of data used for machine learning is usually
                        raw, which can be categorized into different types, such
                        as numerical, categorical, text, and time series data
                        sets.
                      </span>
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </section>

          <div
            style="height:40px"
            aria-hidden="true"
            class="wp-block-spacer"
          ></div>

          <h3 id="cross-industry-standard-process-for-data-mining">
            Cross Industry Standard Process for Data Mining (CRISP-DM)
          </h3>

          <p>
            The CRISP-DM process serves as the foundation for nearly all data
            science processes, and comprises of six sequential steps, including:
          </p>

          <p>
            <strong>Business understanding<br /></strong>This phase entails
            understanding particular business objectives before determining and
            setting up data mining goals. You’ll also determine whether the
            needed resources are available to meet the set project requirements,
            as well as perform a cost-benefit analysis on the whole project
            plan.
          </p>

          <figure class="wp-block-image size-large">
            <img
              loading="lazy"
              width="1024"
              height="1002"
              src="/images/uploads/sites/5/2022/10/1728-1-1024x1002.png"
              alt=""
              class="wp-image-25898"
              srcset="
                /images/uploads/sites/5/2022/10/1728-1-1024x1002.png 1024w,
                /images/uploads/sites/5/2022/10/1728-1-300x293.png    300w,
                /images/uploads/sites/5/2022/10/1728-1-768x751.png    768w,
                /images/uploads/sites/5/2022/10/1728-1.png           1918w
              "
              sizes="(max-width: 1024px) 100vw, 1024px"
            />
          </figure>

          <p>
            <strong>Data understanding<br /></strong>After understanding the
            business needs, you’ll need to determine and analyze the data sets
            to be mined, in line with the project goals. This would mean
            describing data in terms of format and field identities, exploring
            data through visualization, and verifying the same to enhance
            quality consistency.
          </p>

          <p>
            <strong>Data preparation</strong><br />Data preparation, also known
            as data munging in the CRISP-DM process follows these steps:
          </p>

          <ul>
            <li>Data selection</li>
            <li>Data cleaning</li>
            <li>Data construction</li>
            <li>Data integration</li>
            <li>Data formatting</li>
          </ul>

          <p>
            <strong>Modeling</strong><br />This phase entails building and
            assessing multiple data models. It include four steps:
          </p>

          <ul>
            <li>
              Model technique selection based on neural net or regression
              algorithms
            </li>
            <li>
              Test design generation by splitting data into training, test, and
              validation sets
            </li>
            <li>Model development using a preferred code language</li>
            <li>Model assessment based on domain knowledge</li>
          </ul>

          <p>
            <strong>Evaluation</strong><br />This phase evaluates whether the
            constructed model is in line with the forgoing business needs and
            requirements. Besides evaluating the results in the previous phase,
            you’ll also need to review the entire process and ensure that they
            were correctly executed. After that, you’ll be in a better position
            to determine which next steps to follow, whether its deployment,
            further iteration or even start an entirely new project altogether.
          </p>

          <p>
            <strong>Deployment</strong><br />Deployment depends on the
            prevailing business requirements. It can be as simple as coming up
            with a generalized report or as complex as initiating multiple data
            mining processes. Either way, you’ll need to plan, monitor, review,
            and offer ongoing maintenance.
          </p>

          <!-- Flexible content for event category -->
          <!-- END Flexible content for event category -->
        </article>

        <div
          class="post-actions d-flex flex-wrap justify-content-end mb-3 mb-lg-5"
        >
          <div class="post-sharer flex-align-center">
            <span class="txt-caption cl-muted mr-3 text-uppercase">Share</span>
            <div class="a2a_kit flex-align-center">
              <a
                title="Share to Facebook"
                style="color: #3B63B7;"
                class="btn-share mr-3 a2a_button_facebook"
              >
                <svg class="svg-icon">
                  <use xlink:href="#icon-facebook-square"></use>
                </svg>
              </a>
              <a
                title="Share to Twitter"
                style="color: #60A5FC;"
                class="btn-share mr-3 a2a_button_twitter"
              >
                <svg class="svg-icon">
                  <use xlink:href="#icon-twitter"></use>
                </svg>
              </a>
              <a
                title="Share to LinkedIn"
                style="color: #2867B2;"
                class="btn-share mr-3 a2a_button_linkedin"
              >
                <svg class="svg-icon">
                  <use xlink:href="#icon-linkedin"></use>
                </svg>
              </a>
            </div>
          </div>
        </div>
      </div>

      <div class="col-lg-3 ml-xl-auto mt-lg-n3 offset-lg-0">
        <aside class="sticky-sidebar sticky-md pt-md-3">
          <div class="d-none d-lg-block">
            <div class="txt-ttl-5 cl-black mb-3">
              Table of content
            </div>

            <nav id="content-table" class="side-nav mod-simple">
              <ul class="nav nav-pills list-reset">
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#data-preparation-for-machine-learning"
                    >What is Data Preparation for Machine Learning?</a
                  >
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#machine-learning-definition-goals-types"
                    >Machine Learning Definition, Goals, and Types</a
                  >
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#data-preparation-for-machine-learning-best-practices"
                    >How to Prepare Data for Machine Learning - Best
                    Practices</a
                  >
                </li>
                <li class="nav-item">
                  <a target="_self" class="nav-link" href="#sum-up">Sum Up</a>
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#faq-dataset-for-ml-on-data-warehouse"
                    >FAQs on Dataset for Machine Learning on Data Warehouse</a
                  >
                </li>
                <li class="nav-item">
                  <a
                    target="_self"
                    class="nav-link"
                    href="#cross-industry-standard-process-for-data-mining"
                    >Cross Industry Standard Process for Data Mining
                    (CRISP-DM)</a
                  >
                </li>
              </ul>
            </nav>
          </div>
        </aside>
      </div>
    </div>
  </div>
</section>
