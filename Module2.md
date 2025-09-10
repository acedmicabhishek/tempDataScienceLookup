# MODULE-II
## STATISTICAL ANALYSIS

### 1. Introduction to Statistics
Statistics is a branch of mathematics that deals with the collection, analysis, interpretation, presentation, and organization of data. It provides the tools and techniques to understand data, make inferences, and draw conclusions. In data science, statistics is a fundamental tool for understanding data, building predictive models, and evaluating their performance.

### 2. Statistical and Non-statistical Analysis
- **Statistical Analysis:** Involves collecting and analyzing data to identify patterns and trends. It is a scientific method that uses data to make decisions and predictions. For example, using a t-test to determine if there is a significant difference between the means of two groups.
- **Non-statistical Analysis:** Involves analyzing data without using statistical methods. It is often based on intuition, experience, and domain knowledge. For example, a doctor diagnosing a patient based on their symptoms and medical history.

### 3. Major Categories of Statistics
- **Descriptive Statistics:** Summarizes the main features of a dataset. It includes measures of central tendency (mean, median, mode) and measures of dispersion (variance, standard deviation).
- **Inferential Statistics:** Makes inferences about a population based on a sample of data. It includes hypothesis testing, confidence intervals, and regression analysis.

### 4. Population and Sample
- **Population:** The entire group of individuals or objects that you want to study.
- **Sample:** A subset of the population that is selected for analysis. The sample should be representative of the population so that the conclusions drawn from the sample can be generalized to the population.

### 5. Measure of Central Tendency and Dispersion
- **Measures of Central Tendency:** Describe the center of a dataset.
    - **Mean:** The average of all the values in the dataset.
        - Formula: 

         $$ \mu = \frac{\sum_{i=1}^{N} x_i}{N} $$ (for population), $$ \bar{x} = \frac{\sum_{i=1}^{n} x_i}{n} $$ 
         (for sample)
    - **Median:** The middle value in the dataset when the values are arranged in order.
    - **Mode:** The value that appears most frequently in the dataset.
- **Measures of Dispersion:** Describe the spread of a dataset.
    - **Variance:** The average of the squared differences from the mean.
        - Formula: 

        $$ \sigma^2 = \frac{\sum_{i=1}^{N} (x_i - \mu)^2}{N} $$ (for population), $$ s^2 = \frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n-1} $$
         (for sample)
    - **Standard Deviation:** The square root of the variance.
        - Formula:

         $$ \sigma = \sqrt{\frac{\sum_{i=1}^{N} (x_i - \mu)^2}{N}} $$ (for population), $$ s = \sqrt{\frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n-1}} $$ 
         (for sample)

### 6. Moments, Skewness and Kurtosis
- **Moments:** A quantitative measure of the shape of a set of points. The first moment is the mean, the second moment is the variance, the third moment is the skewness, and the fourth moment is the kurtosis.
- **Skewness:** A measure of the asymmetry of the probability distribution of a real-valued random variable about its mean.
    - Formula:
    
     $$ S_k = \frac{E[(X - \mu)^3]}{(\sigma^2)^{3/2}} $$

- **Kurtosis:** A measure of the "tailedness" of the probability distribution of a real-valued random variable.
    - Formula: 
    $$ K = \frac{E[(X - \mu)^4]}{(\sigma^2)^2} $$

### 7. Correlation and Regression
- **Correlation:** A statistical measure that expresses the extent to which two variables are linearly related.
    - Formula (Pearson correlation coefficient):
    
     $$ r = \frac{\sum_{i=1}^{n} (x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum_{i=1}^{n} (x_i - \bar{x})^2 \sum_{i=1}^{n} (y_i - \bar{y})^2}} $$

- **Regression:** A statistical method that allows you to examine the relationship between two or more variables of interest.
    - Formula (Simple Linear Regression):
     $$ y = \beta_0 + \beta_1 x + \epsilon $$

### 8. Theoretical Distributions – Binomial, Poisson, Normal
- **Binomial Distribution:** A discrete probability distribution that describes the number of successes in a sequence of n independent experiments.
    - Formula: 
    $$ P(X=k) = \binom{n}{k} p^k (1-p)^{n-k} $$

- **Poisson Distribution:** A discrete probability distribution that expresses the probability of a given number of events occurring in a fixed interval of time or space.
    - Formula: 
    
    $$ P(X=k) = \frac{\lambda^k e^{-\lambda}}{k!} $$

- **Normal Distribution:** A continuous probability distribution that is symmetrical around the mean. It is also known as the bell curve.
    - Formula (Probability Density Function):
    
     $$ f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{1}{2}(\frac{x-\mu}{\sigma})^2} $$





