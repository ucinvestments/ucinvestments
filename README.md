# UC Investments Dashboard

<style>
  /* Import fonts */
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&display=swap');

  /* Main table styling */
  .repo-table {
    width: 100%;
    border-collapse: separate;
    border-spacing: 0;
    margin: 1.5rem 0;
    font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
    border-radius: 0.75rem;
    overflow: hidden;
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -2px rgba(0, 0, 0, 0.1);
    border: 1px solid #e2e8f0;
  }

  .repo-table th {
    background: linear-gradient(135deg, #003262, #3B7EA1);
    color: white;
    font-family: 'Space Grotesk', sans-serif;
    text-align: center;
    padding: 1rem;
    font-weight: 600;
    letter-spacing: -0.01em;
  }

  .repo-table td {
    padding: 0.75rem 1rem;
    text-align: center;
    border-bottom: 1px solid #e2e8f0;
    transition: all 0.2s ease;
  }

  .repo-table tr:last-child td {
    border-bottom: none;
  }

  .repo-table tr:nth-child(even) {
    background-color: #f8fafc;
  }

  .repo-table tr:hover td {
    background-color: rgba(251, 213, 21, 0.1);
  }

  .repo-name {
    font-weight: 600;
    color: #003262;
    text-decoration: none;
    transition: color 0.2s ease;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.5rem;
  }

  .repo-name:hover {
    color: #3B7EA1;
    text-decoration: underline;
  }

  .repo-name svg {
    width: 18px;
    height: 18px;
  }

  .badge {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    border-radius: 9999px;
    font-size: 0.875rem;
    font-weight: 500;
    transition: transform 0.2s ease;
    text-decoration: none;
  }

  .badge:hover {
    transform: translateY(-1px);
  }

  .badge img {
    border-radius: 4px;
  }

  .summary-badges {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
    justify-content: center;
    margin: 2rem 0;
  }

  .summary-badge {
    display: inline-block;
    transition: transform 0.2s ease;
  }

  .summary-badge:hover {
    transform: translateY(-2px);
  }

  .dashboard-title {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 2rem;
    font-weight: 700;
    text-align: center;
    margin-bottom: 1.5rem;
    color: #003262;
    letter-spacing: -0.02em;
    padding-bottom: 0.5rem;
    border-bottom: 3px solid #FDB515;
    width: fit-content;
    margin-left: auto;
    margin-right: auto;
  }
</style>

<h1 class="dashboard-title">UC Investments Dashboard</h1>

<table class="repo-table">
  <thead>
    <tr>
      <th>Repository</th>
      <th>Open Issues</th>
      <th>Closed Issues</th>
      <th>Pull Requests</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <a href="https://github.com/ucinvestments/UC-wages" class="repo-name">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor">
            <path d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"/>
          </svg>
          UC-wages
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/UC-wages/issues" class="badge">
          <img src="https://img.shields.io/github/issues/ucinvestments/UC-wages?color=blue&style=flat-square" alt="Open issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/UC-wages/issues?q=is%3Aissue+is%3Aclosed" class="badge">
          <img src="https://img.shields.io/github/issues-closed/ucinvestments/UC-wages?color=success&style=flat-square" alt="Closed issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/UC-wages/pulls" class="badge">
          <img src="https://img.shields.io/github/issues-pr/ucinvestments/UC-wages?color=orange&style=flat-square" alt="Pull requests">
        </a>
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://github.com/ucinvestments/BDS" class="repo-name">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor">
            <path d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"/>
          </svg>
          BDS
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/BDS/issues" class="badge">
          <img src="https://img.shields.io/github/issues/ucinvestments/BDS?color=blue&style=flat-square" alt="Open issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/BDS/issues?q=is%3Aissue+is%3Aclosed" class="badge">
          <img src="https://img.shields.io/github/issues-closed/ucinvestments/BDS?color=success&style=flat-square" alt="Closed issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/BDS/pulls" class="badge">
          <img src="https://img.shields.io/github/issues-pr/ucinvestments/BDS?color=orange&style=flat-square" alt="Pull requests">
        </a>
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://github.com/ucinvestments/UC-Investments" class="repo-name">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor">
            <path d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"/>
          </svg>
          UC-Investments
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/UC-Investments/issues" class="badge">
          <img src="https://img.shields.io/github/issues/ucinvestments/UC-Investments?color=blue&style=flat-square" alt="Open issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/UC-Investments/issues?q=is%3Aissue+is%3Aclosed" class="badge">
          <img src="https://img.shields.io/github/issues-closed/ucinvestments/UC-Investments?color=success&style=flat-square" alt="Closed issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/UC-Investments/pulls" class="badge">
          <img src="https://img.shields.io/github/issues-pr/ucinvestments/UC-Investments?color=orange&style=flat-square" alt="Pull requests">
        </a>
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://github.com/ucinvestments/holdings" class="repo-name">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor">
            <path d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"/>
          </svg>
          holdings
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/holdings/issues" class="badge">
          <img src="https://img.shields.io/github/issues/ucinvestments/holdings?color=blue&style=flat-square" alt="Open issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/holdings/issues?q=is%3Aissue+is%3Aclosed" class="badge">
          <img src="https://img.shields.io/github/issues-closed/ucinvestments/holdings?color=success&style=flat-square" alt="Closed issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/holdings/pulls" class="badge">
          <img src="https://img.shields.io/github/issues-pr/ucinvestments/holdings?color=orange&style=flat-square" alt="Pull requests">
        </a>
      </td>
    </tr>
    <tr>
      <td>
        <a href="https://github.com/ucinvestments/people" class="repo-name">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" fill="currentColor">
            <path d="M2 2.5A2.5 2.5 0 014.5 0h8.75a.75.75 0 01.75.75v12.5a.75.75 0 01-.75.75h-2.5a.75.75 0 110-1.5h1.75v-2h-8a1 1 0 00-.714 1.7.75.75 0 01-1.072 1.05A2.495 2.495 0 012 11.5v-9zm10.5-1V9h-8c-.356 0-.694.074-1 .208V2.5a1 1 0 011-1h8zM5 12.25v3.25a.25.25 0 00.4.2l1.45-1.087a.25.25 0 01.3 0L8.6 15.7a.25.25 0 00.4-.2v-3.25a.25.25 0 00-.25-.25h-3.5a.25.25 0 00-.25.25z"/>
          </svg>
          people
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/people/issues" class="badge">
          <img src="https://img.shields.io/github/issues/ucinvestments/people?color=blue&style=flat-square" alt="Open issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/people/issues?q=is%3Aissue+is%3Aclosed" class="badge">
          <img src="https://img.shields.io/github/issues-closed/ucinvestments/people?color=success&style=flat-square" alt="Closed issues">
        </a>
      </td>
      <td>
        <a href="https://github.com/ucinvestments/people/pulls" class="badge">
          <img src="https://img.shields.io/github/issues-pr/ucinvestments/people?color=orange&style=flat-square" alt="Pull requests">
        </a>
      </td>
    </tr>
  </tbody>
</table>

<div class="summary-badges">
  <a href="https://github.com/search?q=org%3Aucinvestments+is%3Aissue+is%3Aopen&type=issues" class="summary-badge">
    <img src="https://img.shields.io/github/issues-search/ucinvestments?query=is%3Aissue+is%3Aopen+user%3Aucinvestments&label=All%20Open%20Issues&style=for-the-badge&color=003262" alt="All Open Issues">
  </a>
  
  <a href="https://github.com/search?q=org%3Aucinvestments+is%3Aissue+is%3Aopen+label%3A%22in+progress%22&type=issues" class="summary-badge">
    <img src="https://img.shields.io/github/issues-search/ucinvestments?query=is%3Aissue+is%3Aopen+user%3Aucinvestments+label%3A%22in+progress%22&label=In%20Progress&style=for-the-badge&color=FDB515" alt="In Progress">
  </a>
  
  <a href="https://github.com/search?q=org%3Aucinvestments+is%3Aissue+is%3Aclosed+closed%3A%3E2025-09-01&type=issues" class="summary-badge">
    <img src="https://img.shields.io/github/issues-search/ucinvestments?query=is%3Aissue+is%3Aclosed+user%3Aucinvestments+closed%3A%3E2025-09-01&label=Recently%20Closed&style=for-the-badge&color=3B7EA1" alt="Recently Closed">
  </a>
</div>
