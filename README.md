# README: Bias Audit and Fairness Mitigation in Income Prediction

## Project Overview

This project conducts a comprehensive **bias audit** on the widely used **Adult Income Dataset** from the UCI Machine Learning Repository. The dataset is commonly employed to predict whether an individual earns more than $50K per year based on attributes such as age, education, occupation, race, and gender. The primary goal of this audit is to:

- **Identify potential biases** in income predictions, particularly across **gender and racial groups**.
- **Quantify fairness metrics**, including statistical parity and disparate impact.
- **Apply mitigation techniques** like reweighing and disparate impact removal to reduce unfairness.
- **Evaluate trade-offs** between fairness and model accuracy.

The project also aligns with broader **ethical principles**, emphasizing fairness, accountability, transparency, and respect for human rights in AI systems.

---

## Key Findings

### Bias Patterns
1. **Gender Bias**:
   - Males earning >$50K: **30.6%**
   - Females earning >$50K: **10.9%**
   - **Statistical Parity Difference**: -0.199 (indicating significant disparity)
   - **Disparate Impact**: 0.35 (well below the fairness threshold of 0.8)

2. **Racial Bias**:
   - Whites earning >$50K: **25.6%**
   - Blacks earning >$50K: **12.4%**
   - **Statistical Parity Difference**: -0.131
   - **Disparate Impact**: 0.48

### Mitigation Strategies and Results
- **Reweighing (Gender Bias)**:
  - Adjusted instance weights to balance outcomes.
  - **Accuracy improved to 95.9%**.
  - **Fairness improved**: Average Odds Difference reduced to -0.015.

- **Disparate Impact Remover (Race Bias)**:
  - Repaired features to reduce racial bias.
  - **Accuracy**: 86.9%.
  - **Fairness improved**: Disparate Impact increased to 0.32.

---

## Ethical Implications

The findings of this project highlight the **real-world consequences** of biased AI systems, including:
- **Unfair income predictions** reinforcing systemic inequalities.
- **Biased hiring, lending, and insurance decisions** leading to legal and ethical issues.
- **Erosion of public trust** in AI systems due to lack of transparency and fairness.

The project aligns with the following **ethical principles**:
- **Fairness and Non-Discrimination**: Addressing disparities through technical interventions like reweighing and disparate impact removal.
- **Accountability and Transparency**: Measuring and reporting fairness metrics to ensure responsible AI development.
- **Respect for Human Rights**: Ensuring AI systems do not infringe on fundamental rights, such as the right to non-discrimination.
- **Continuous Improvement**: Emphasizing the need for ongoing monitoring and stakeholder engagement.

---

## Recommendations for Stakeholders

To ensure fairness in AI systems, stakeholders should:
1. **Refine Feature Engineering**:
   - Remove or transform sensitive attributes (e.g., race, gender) using fairness-aware techniques like **Disparate Impact Remover**.
   
2. **Use Reweighing During Training**:
   - Balance the influence of privileged and unprivileged groups to improve fairness without sacrificing accuracy.

3. **Monitor Fairness Metrics Continuously**:
   - Track **Statistical Parity Difference**, **Disparate Impact**, and **Average Odds Difference** throughout the model lifecycle.

4. **Incorporate Fairness into Model Selection**:
   - Choose models based not only on accuracy but also on fairness performance across demographic groups.

5. **Engage in Context-Sensitive Evaluation**:
   - Recognize that algorithmic solutions alone are insufficient; societal and organizational measures are equally important.

---

## Project Structure

The project includes the following components:
1. **Bias Audit Presentation (PPT)**: Summarizes key findings, mitigation strategies, and real-world implications.
2. **Ethics Statement (PDF)**: Explores the broader ethical principles guiding the project, including fairness, accountability, and transparency.
3. **Code and Data**: Scripts for bias detection, mitigation, and evaluation (not included in the provided files but assumed as part of the project).

---

## How to Use This Project

### For Researchers
- Review the **bias audit findings** to understand disparities in the dataset.
- Explore the **mitigation techniques** (reweighing, disparate impact removal) and their effectiveness.
- Use the **fairness metrics** as a benchmark for evaluating other models.

### For Developers
- Implement the recommended **fairness-aware techniques** in your own models.
- Continuously monitor **fairness metrics** during model development and deployment.
- Refer to the **ethical guidelines** to ensure responsible AI practices.

### For Policymakers
- Understand the **real-world implications** of biased AI systems.
- Advocate for **transparency and accountability** in AI development.
- Promote **regulatory frameworks** that prioritize fairness and non-discrimination.

---

## Conclusion

This project underscores the **importance of auditing and mitigating bias** in machine learning models. Key takeaways include:
- **Significant biases** exist in income predictions across gender and racial groups.
- **Fairness metrics** like Statistical Parity Difference and Disparate Impact are critical for quantifying disparities.
- **Mitigation techniques** can improve fairness while maintaining model performance.
- **Ensuring fairness** is not just a technical challenge but a **social responsibility**.

By addressing these issues, we can work toward AI systems that promote **equity, trust, and inclusion** in society.

---

## References

- Barocas, S., Hardt, M., & Narayanan, A. (2019). *Fairness and Machine Learning*. fairmlbook.org.
- European Commission. (2019). *Ethics Guidelines for Trustworthy AI*.
- Floridi, L., Cowls, J., Beltrametti, M., et al. (2018). *AI4People—An Ethical Framework for a Good AI Society*.
- IEEE. (2019). *Ethically Aligned Design: A Vision for Prioritizing Human Well-being with Autonomous and Intelligent Systems*.
- Jobin, A., Ienca, M., & Vayena, E. (2019). *The global landscape of AI ethics guidelines*.
- United Nations. (2021). *Universal Declaration of Human Rights*.

---

## Contact

For questions or further information, please contact the project team.  
**Email**: [mavundlatm@icloud.com]  
**GitHub**: [[Your Repository Link](https://github.com/Thabo-Mavundla)]  

---

