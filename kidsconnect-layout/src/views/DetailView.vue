<template>
  <div>
    <Header />
    <div class="container">
      <div class="top-nav">
        <router-link to="/" class="btn btn-outline back-btn">← Назад</router-link>
        <button class="btn btn-outline map-btn">На карте 📍</button>
      </div>
      
      <div class="detail-card">
        <div class="detail-header-row">
          <h1 class="detail-title">Легкая атлетика (в Юбилейном мкр)</h1>
          <button class="btn btn-primary">Записаться</button>
        </div>

        <div class="detail-main-info">
          <div class="detail-img">
             <svg width="64" height="64" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
          </div>
          <div class="detail-text">
            <span class="badge badge-red" style="margin-bottom: 12px; display: inline-block;">Набор открыт</span>
            <p><span class="icon">👤</span> 10-18 лет</p>
            <p><span class="icon">📍</span> г. Иркутск, Юбилейный мкр, стр. 49/1</p>
            <p><span class="icon">🏢</span> ФОК "Юбилейный"</p>
          </div>
        </div>

        <div class="detail-grid">
          <div class="grid-col">
            <h4 class="grid-title">ГРУППЫ</h4>
            <p class="grid-text">Этап начальной подготовки</p>
            <p class="grid-text">Тренер: Иванов А.А.</p>
          </div>
          <div class="grid-col">
            <h4 class="grid-title">РАСПИСАНИЕ ЗАНЯТИЙ</h4>
            <p class="grid-text">Пн, Вт, Чт, Сб</p>
            <div class="time-tags">
              <span class="time-tag">08:00 - 10:00</span>
              <span class="time-tag">18:00 - 19:30</span>
            </div>
          </div>
        </div>

        <div class="detail-description">
          <h4 class="grid-title">ОПИСАНИЕ</h4>
          <p class="desc-text">Легкая атлетика - олимпийский вид спорта, объединяющий бег, прыжки, метания и ходьбу. Занятия развивают выносливость, силу, скорость и координацию.</p>
        </div>

        <!-- Аккордеон -->
        <div class="accordion">
          <div class="accordion-header" @click="isOpen = !isOpen">
            <h4 class="grid-title" style="margin: 0;">СОДЕРЖАНИЕ ПРОГРАММЫ</h4>
            <span>{{ isOpen ? '▲' : '▼' }}</span>
          </div>
          <div class="accordion-body" v-show="isOpen">
            <p class="acc-subtitle">Базовый уровень</p>
            <ul class="acc-list">
              <li>Базовый уровень сложности: первый этап подготовки.</li>
              <li>Обязательные предметные области: физическая культура.</li>
              <li>Теория и методика физической культуры.</li>
            </ul>
            <p class="acc-subtitle" style="margin-top: 16px;">Углубленный уровень</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import Header from '../components/Header.vue'

const isOpen = ref(true)
</script>

<style scoped>
.top-nav {
  display: flex;
  justify-content: space-between;
  margin: 20px 0;
}
.back-btn { background: white; }

.detail-card {
  background: white;
  border-radius: 4px;
  padding: 32px;
  border: 1px solid var(--border-color);
}

.detail-header-row {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 24px;
}
.detail-title { font-size: 22px; font-weight: 600; }

.detail-main-info {
  display: flex;
  gap: 32px;
  margin-bottom: 32px;
}
.detail-img {
  width: 240px;
  height: 160px;
  background: #C4C4C4;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.detail-text p {
  font-size: 14px;
  margin-bottom: 8px;
  color: var(--text-main);
  display: flex;
  align-items: center;
}
.detail-text .icon {
  width: 24px;
  color: #666;
}

.detail-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  padding: 24px 0;
  border-top: 1px solid var(--border-color);
  border-bottom: 1px solid var(--border-color);
  margin-bottom: 24px;
}
.grid-title {
  font-size: 12px;
  font-weight: 700;
  color: var(--text-muted);
  text-transform: uppercase;
  margin-bottom: 12px;
  letter-spacing: 0.5px;
}
.grid-text { font-size: 14px; margin-bottom: 8px; }

.detail-description { margin-bottom: 32px; }
.desc-text {
  font-size: 14px;
  color: var(--text-main);
  line-height: 1.5;
}

/* Аккордеон */
.accordion {
  background: #FAFAFA;
  border-radius: 4px;
  padding: 16px 24px;
  border: 1px solid var(--border-color);
}
.accordion-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer;
}
.accordion-body { margin-top: 16px; }
.acc-subtitle { font-size: 14px; font-weight: 600; margin-bottom: 8px; }
.acc-list {
  list-style-type: disc;
  padding-left: 20px;
  font-size: 14px;
  color: var(--text-main);
  line-height: 1.6;
}
</style>