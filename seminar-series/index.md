---
layout: default
title: Seminar Series
permalink: /seminar-series/
---

<div class="seminar-page">
  <h1>Seminar Series</h1>
  <p>A bi-weekly public seminar on the Data Foundations of AI.</p>

  <div class="seminar-info-grid">
    <div class="info-card">
      <h3>📅 Format</h3>
      <ul>
        <li>45 minutes: invited talk</li>
        <li>15 minutes: Q&A</li>
      </ul>
    </div>
<!--     <div class="info-card">
      <h3>🕐 Default Time</h3>
      <p>Tuesday 6 PM UTC</p>
    </div> -->
    <div class="info-card">
      <h3>🎙️ Nominate a Speaker</h3>
      <p><a href="https://forms.gle/DV92KecS9RsQGFj96" class="text-link">Submit nomination form</a></p>
    </div>
  </div>

  <h2 class="section-title">📅 Upcoming Seminars</h2>
  <p>To add these seminars to your Google Calendar, please click <a href=https://calendar.google.com/calendar/u/1?cid=Y180MzA4NmNkYTAyZTZkYjEyNDZiNTU0ZWNkYjhiODE3ZTZmODQ0YmRhNjRiNzI1ZmJkNjRkOTgxMTU3ZWY2N2FlQGdyb3VwLmNhbGVuZGFyLmdvb2dsZS5jb20 class="text-link">this link </a>.</p>
  <div class="seminar-calendar">
    <table class="seminar-table">
      <thead>
        <tr>
          <th>Time</th>
          <th>Speaker</th>
          <th>Topic</th>
          <th>Host</th>
          <th>Link</th>
        </tr>
      </thead>
      <tbody>
        <tr class="expandable-row" onclick="toggleDetails('seminar-1')">
          <td>7 PM UTC | 2 PM ET<br>Mar 3, 2026</td>
          <td><a href="https://dylanzsz.github.io/" onclick="event.stopPropagation()">Dylan Zhang</a></td>
          <td>More Fruitful SFT by Respecting The Learner's Distribution <span class="expand-indicator">▼</span></td>
          <td>Junwei</td>
          <td onclick="event.stopPropagation()"><span class="status-pending">TBA</span></td>
        </tr>
        <tr class="details-row" id="seminar-1" style="display: none;">
          <td colspan="5">
            <div class="seminar-details">
              <div class="speaker-photo">
                <img src="{{ '/assets/images/seminars/dylan-zhang.jpg' | relative_url }}" alt="Dylan Zhang">
              </div>
              <div class="seminar-content">
                <h3>More Fruitful SFT by Respecting The Learner's Distribution</h3>
                
                <h4>Abstract</h4>
                <p>Classic supervised fine-tuning (SFT) ignores the learner. It treats supervision as universally valid, even when the training data differs substantially from what the model itself would produce — a mismatch that has proven troublesome for LLM post-training in a variety of ways. Recent work on on-policy distillation and self-distillation fine-tuning has similarly argued that effective supervision must respect the learner's own policy.</p>
                
                <p>In this talk, I present two works built around that single principle: supervision should be aligned with the learner's distribution. Both implement it as a simple modification to standard SFT.</p>
                
                <p><strong>GRAPE</strong> addresses this from a data selection perspective. For each instruction, it selects the response with the highest probability under the target model from a pool of existing candidates, using only a forward pass. Models trained on GRAPE-curated data outperform multiple strong baselines while being lightweight and scalable.</p>
                
                <p>When SFT is followed by online RL, we show that stronger SFT (and variants) checkpoints can paradoxically underperform weaker ones after RL — because standard SFT optimizes for offline performance in isolation, without accounting for the on-policy distribution that RL will explore during its own rollouts.</p>
                
                <p><strong>PEAR</strong> extends this idea to the setting where SFT is followed by online RL. We first show that stronger SFT checkpoints can paradoxically underperform weaker ones after RL — because standard SFT optimizes for offline performance in isolation, without accounting for the on-policy distribution that RL will later explore. PEAR addresses this by reweighting the loss on each response according to its importance weight: how likely the target policy is to produce that response. We further show that this correction can operate at finer granularities, reweighting individual tokens based on how likely the continuation from that point in the offline data would be under the target policy. This importance-sampling correction, inspired by off-policy evaluation in RL, bridges the gap between the static SFT dataset and the dynamic on-policy distribution, yielding consistent post-RL gains.</p>
                
                <p>Both methods operationalize the same insight — that effective supervision must be shaped by the learner's own distribution — through complementary mechanisms: GRAPE by selecting responses the model trains on, PEAR by reweighting how much it learns. Together, they demonstrate that simple, policy-aware corrections can improve the effectiveness of SFT.</p>
                
                <h4>Bio</h4>
                <p>Dylan Zhang is a Ph.D. student in Computer Science at the University of Illinois Urbana-Champaign (UIUC), advised by Prof. Hao Peng. His research focuses on large language model (LLM) post-training, particularly on developing offline training algorithms for efficient and effective model alignment. More broadly, he is interested in understanding the behavior, generalization, and inductive biases of large language models—how they learn from data, adapt through supervision, and exhibit emergent capabilities.</p>
              </div>
            </div>
          </td>
        </tr>
        <tr>
          <td>Mar 10, 2026</td>
          <td><a href="https://nick11roberts.science/">Nicholas Roberts</a></td>
          <td>Scaling Laws and Evaluation</td>
          <td>Brian</td>
          <td><span class="status-pending">TBA</span></td>
        </tr>
        <tr>
          <td>Mar 24, 2026</td>
          <td><a href="https://mayeechen.github.io/">Mayee Chen</a></td>
          <td>Data Mixing</td>
          <td>Brian</td>
          <td><span class="status-pending">TBA</span></td>
        </tr>
        <tr>
          <td>Apr 7, 2026</td>
          <td><a href="https://lumos23.github.io/">Luxi He</a></td>
          <td>Data in LLM Lifecycles</td>
          <td>Junwei</td>
          <td><span class="status-pending">TBA</span></td>
        </tr>
        <tr>
          <td>Apr 21, 2026</td>
          <td><a href="https://zhenghaizhong.com/">Haizhong Zheng</a></td>
          <td>Efficient RL for LLMs</td>
          <td>Brian</td>
          <td><span class="status-pending">TBA</span></td>
        </tr>
      </tbody>
    </table>
  </div>

  <script>
    function toggleDetails(id) {
      const detailsRow = document.getElementById(id);
      const expandableRow = detailsRow.previousElementSibling;
      const indicator = expandableRow.querySelector('.expand-indicator');
      
      if (detailsRow.style.display === 'none') {
        detailsRow.style.display = 'table-row';
        indicator.textContent = '▲';
      } else {
        detailsRow.style.display = 'none';
        indicator.textContent = '▼';
      }
    }
  </script>

  <div class="calendar-note">
    <p><strong>Note:</strong> Times are provided in UTC and ET. Convert to your timezone before joining. Zoom links will be shared closer to the event date.</p>
  </div>

  <h2 class="section-title">📚 Past Seminars</h2>
  <div class="past-seminars">
    <table class="seminar-table">
      <thead>
        <tr>
          <th>Date</th>
          <th>Speaker</th>
          <th>Topic</th>
          <th>Host</th>
          <th>Recording</th>
        </tr>
      </thead>
      <tbody>
        <tr class="no-data">
          <td colspan="5">Past seminars will be listed here after our first event.</td>
        </tr>
      </tbody>
    </table>
  </div>

  <div class="recordings-note">
    <p><em>We record talks when speakers consent. Recordings will be made available here.</em></p>
  </div>
</div>
