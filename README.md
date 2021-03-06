In this project, I used Python to automate the downloading of company's updated annual report from <a href="https://www.sec.gov/edgar/searchedgar/companysearch.html" target="_blank">SEC website</a>. The annual report will be downloaded as XBRL instance document.

To view the project <code>Download_company_updated_annual_report_XBRL.ipynb</code>, click <a href="https://nbviewer.jupyter.org/github/steffen-zou/Download-updated-company-annual-report-XBRL/blob/master/Download_company_updated_annual_report_XBRL.ipynb">here</a> which will display the project using Jupyter Notebook Viewer, as GitHub sometimes is not able to load this project.

The <code>stock_db_dump.sql</code> file is a PostgreSQL database backup that contains a table that this project selects from. The command to restore the backup can be found in the <a href="https://www.postgresql.org/docs/8.1/backup.html#BACKUP-DUMP-RESTORE">PostgreSQL documentation</a>.

Below is the description of each column from the table that this project selects from.

<table>
  <thead>
    <tr>
      <th>Column</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>company_name</td>
      <td>Company name</td>
    </tr>
    <tr>
      <td>filings</td>
      <td>The type of filing that the financials data is retrieved from (e.g. 10-K, 20-F, 40-F)</td>
    </tr>
    <tr>
      <td>reporting_currency</td>
      <td>Reporting currency</td>
    </tr>
    <tr>
      <td>fiscal_year_ended</td>
      <td>Fiscal year ended</td>
    </tr>
    <tr>
      <td>cash_and_equivalents</td>
      <td>Cash and cash equivalents</td>
    </tr>
    <tr>
      <td>short_term_investments</td>
      <td>Short-term investments</td>
    </tr>
    <tr>
      <td>current_debt</td>
      <td>Current portion of debt/notes</td>
    </tr>
    <tr>
      <td>revenue</td>
      <td>Revenue</td>
    </tr>
    <tr>
      <td>cost_of_revenue</td>
      <td>Cost of revenue</td>
    </tr>
    <tr>
      <td>revenue_1_fy_ago</td>
      <td>Revenue from one fiscal year ago</td>
    </tr>
    <tr>
      <td>operating_cash_flow</td>
      <td>Operating cash flow</td>
    </tr>
    <tr>
      <td>capital_expenditure</td>
      <td>Capital expenditure. It consists of the following items under "Cash flows from investing activities": 
        <ul>
          <li>Purchases of property, plant and equipment</li>
          <li>Capitalized software development costs</li>
          <li>Capitalized internal-use software</li>
          <li>Purchase of intangible assets</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
