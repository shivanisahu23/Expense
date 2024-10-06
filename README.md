### Expensemanager

**ExpenseManager** is a comprehensive application designed to streamline employee expense management within organizations. It allows employees to easily submit expense claims for various categories such as travel and meals, complete with essential details like date and amount. The app features a robust approval workflow where claims are initially submitted, reviewed by managers, and marked as approved or rejected. With role-based permissions ensuring that only authorized personnel can submit and approve claims, ExpenseManager enhances security and accountability. Additionally, it provides real-time status tracking and valuable insights into expense trends, ultimately increasing efficiency and improving financial management for organizations.

### Installation

You can install this app using the [bench](https://github.com/frappe/bench) CLI:

```bash
cd $PATH_TO_YOUR_BENCH
bench get-app $URL_OF_THIS_REPO --branch develop
bench install-app expensemanager
```

### Contributing

This app uses `pre-commit` for code formatting and linting. Please [install pre-commit](https://pre-commit.com/#installation) and enable it for this repository:

```bash
cd apps/expensemanager
pre-commit install
```

Pre-commit is configured to use the following tools for checking and formatting your code:

- ruff
- eslint
- prettier
- pyupgrade

### CI

This app can use GitHub Actions for CI. The following workflows are configured:

- CI: Installs this app and runs unit tests on every push to `develop` branch.
- Linters: Runs [Frappe Semgrep Rules](https://github.com/frappe/semgrep-rules) and [pip-audit](https://pypi.org/project/pip-audit/) on every pull request.


### License

mit
