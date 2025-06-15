<template>
  <div class="portfolio-container">
    <div class="profile-card">
      <img
        src="https://images.unsplash.com/photo-1486312338219-ce68d2d6f44d?auto=format&fit=facearea&w=256&q=80"
        alt="Your face or logo"
        class="profile-img"
      />
      <h1 class="profile-name">YOUR NAME HERE</h1>
      <p class="profile-title">Frontend Developer</p>
      <p class="profile-description">
        I love creating clean user interfaces and simple web apps!
      </p>
    </div>
    <div class="skills-section">
      <h2 class="section-title">Skills</h2>
      <ul class="skills-list">
        <li class="skill-item">HTML</li>
        <li class="skill-item">CSS</li>
        <li class="skill-item">JavaScript</li>
        <li class="skill-item">React</li>
      </ul>
    </div>
    <div class="project-section">
      <h2 class="section-title">Project</h2>
      <div class="project-card">
        <h3 class="project-name">Project Name</h3>
        <p class="project-summary">Short project summary goes here.</p>
        <a
          href="#"
          target="_blank"
          rel="noopener noreferrer"
          class="project-link"
        >
          View Project
        </a>
      </div>
    </div>
    <div class="contact-section">
      <h2 class="section-title">Contact</h2>
      <p class="contact-email">
        Email:
        <a href="mailto:your.email@example.com" class="contact-email-link">
          your.email@example.com
        </a>
      </p>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.portfolio-container {
  min-height: 100vh;
  background-color: #f8fafc; /* bg-background (ตัวอย่างสีเบื้องต้น) */
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 3rem 1rem; /* px-4 py-12 */
}

.profile-card,
.project-card {
  width: 100%;
  max-width: 28rem; /* max-w-md */
  background-color: #ffffff; /* bg-card */
  border-radius: 0.5rem; /* rounded-lg */
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1), 0 1px 2px rgba(0, 0, 0, 0.06); /* shadow */
  margin-bottom: 2.5rem; /* mb-10 */
  padding: 1.5rem; /* p-6 */
  text-align: center;
}

.profile-img {
  margin: 0 auto 0.75rem auto; /* mx-auto mb-3 */
  width: 5rem; /* w-20 */
  height: 5rem; /* h-20 */
  border-radius: 9999px; /* rounded-full */
  object-fit: cover;
  border: 2px solid #3b82f6; /* border-2 border-primary (ตัวอย่างสี) */
}

.profile-name {
  font-size: 1.5rem; /* text-2xl */
  font-weight: 700; /* font-bold */
  margin-bottom: 0.5rem; /* mb-2 */
}

.profile-title {
  font-size: 1rem; /* text-base */
  color: #64748b; /* text-muted-foreground (ตัวอย่างสี) */
  margin-bottom: 0.5rem; /* mb-2 */
}

.profile-description {
  font-size: 1rem; /* text-base */
}

.skills-section,
.project-section,
.contact-section {
  width: 100%;
  max-width: 28rem; /* max-w-md */
  margin-bottom: 2.5rem; /* mb-10 (สำหรับ skills & project) */
}

.contact-section {
  margin-bottom: 0; /* Remove mb-10 for contact section if it's the last */
}

.section-title {
  font-size: 1.25rem; /* text-xl */
  font-weight: 600; /* font-semibold */
  margin-bottom: 1rem; /* mb-4 */
  text-align: center; /* ส่วนใหญ่ในโค้ดต้นฉบับ skills และ contact มี h2 อยู่ตรงกลาง */
}

.skills-list {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem; /* gap-2 */
  justify-content: center;
  list-style: none; /* Remove default list style */
  padding: 0; /* Remove default padding */
  margin: 0; /* Remove default margin */
}

.skill-item {
  background-color: #3b82f6; /* bg-primary (ตัวอย่างสี) */
  color: #ffffff; /* text-primary-foreground (ตัวอย่างสี) */
  border-radius: 0.25rem; /* rounded */
  padding: 0.25rem 0.5rem; /* px-2 py-1 */
  font-size: 0.875rem; /* text-sm */
}

.project-card {
  text-align: left; /* p-4 text-left */
}

.project-name {
  font-size: 1.125rem; /* text-lg */
  font-weight: 700; /* font-bold */
}

.project-summary {
  color: #64748b; /* text-muted-foreground (ตัวอย่างสี) */
  margin-bottom: 0.5rem; /* mb-2 */
  font-size: 0.875rem; /* text-sm */
}

.project-link,
.contact-email-link {
  color: #3b82f6; /* text-primary (ตัวอย่างสี) */
  text-decoration: underline;
  font-size: 0.875rem; /* text-sm */
}

.contact-email {
  margin-bottom: 0.25rem; /* mb-1 */
}
</style>
