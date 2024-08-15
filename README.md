# Upper Confidence Bound (UCB) Algorithm

This repository contains an implementation of the Upper Confidence Bound (UCB) algorithm, a popular reinforcement learning technique used for solving the multi-armed bandit problem. UCB is used in scenarios where you need to balance the exploration of different actions with the exploitation of the best-known action.

## Contents

- **ucb.py**: The main script that implements the UCB algorithm.
- **data.csv**: The dataset file representing different arms (actions) and their corresponding rewards.
- **results/**: A directory containing visualizations and results of the UCB algorithm's performance.
- **requirements.txt**: A list of Python dependencies required to run the code.

## Implementation Details

The implementation includes the following key steps:

1. **Data Loading**: The dataset (`data.csv`) consists of multiple rounds of interactions with various arms, each providing a reward. The goal is to maximize the cumulative reward over time.
2. **UCB Algorithm**:
    - The UCB algorithm selects an arm (action) based on the upper confidence bound for each arm's expected reward.
    - It balances exploration (trying out less-selected arms) with exploitation (selecting the arm with the highest known reward).
    - At each round, the algorithm updates the selection strategy based on the observed rewards and the number of times each arm has been chosen.
3. **Performance Evaluation**: The results include visualizations of the cumulative reward and the number of times each arm was selected, demonstrating the effectiveness of the UCB algorithm.

## Usage

To use this code, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/mazimum86/UCB.git
    ```
2. Navigate to the repository directory:
    ```bash
    cd UCB
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the UCB algorithm:
    ```bash
    python ucb.py
    ```

## Dependencies

The following Python packages are required to run the code:

- numpy
- matplotlib
- pandas

These dependencies are listed in the `requirements.txt` file and can be installed using `pip`.

## Results

The output includes:

- **Cumulative Reward**: A plot showing the total reward accumulated over time.
- **Arm Selections**: A plot indicating the number of times each arm was selected during the run of the algorithm.

## Contributing

Contributions are welcome! If you have any suggestions for improvements or additional features, feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
