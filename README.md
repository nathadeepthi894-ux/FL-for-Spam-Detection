# FL-for-Spam-Detection
FedSecureXAI is a federated learning framework designed to enable secure and privacy-preserving email spam and phishing detection across multiple organizations. Unlike traditional centralized approaches that require sharing sensitive email data, this system allows collaborative model training while keeping data localized, ensuring compliance with data protection regulations such as GDPR.

The framework combines powerful machine learning techniques with privacy and security enhancements. It uses XGBoost-based local models trained on a comprehensive feature set, including TF-IDF text features, URL structure, and attachment metadata. To protect against privacy attacks, FedSecureXAI incorporates a differential privacy mechanism that adds controlled noise to client updates, preventing information leakage.

A key contribution of the framework is its trust-weighted aggregation method, which selects the most reliable client models based on prediction performance and data contribution. This approach improves robustness, especially in non-IID data settings where traditional methods like FedAvg often fail. Additionally, the system is resilient to adversarial behavior through built-in Byzantine fault tolerance, ensuring stable performance even when some clients act maliciously.

FedSecureXAI also integrates federated SHAP-based explainability, enabling global interpretation of model decisions without exposing raw data. Experimental results on a large multi-source email dataset show that the framework achieves near-centralized performance with minimal loss, even under strict privacy constraints.

Overall, FedSecureXAI provides a scalable, secure, and transparent solution for modern distributed email security systems.
