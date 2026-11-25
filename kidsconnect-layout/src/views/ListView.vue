<template>
  <div>
    <Header />
    <div class="container layout">
      <!-- Левая колонка (Список) -->
      <div class="main-content">
        <!-- Панель поиска -->
        <div class="search-panel">
          <div class="search-input-wrapper">
            <span class="search-icon">🔍</span>
            <input type="text" placeholder="Поиск" />
          </div>
          <div class="radio-group">
            <label><input type="radio" name="pay" checked> Все</label>
            <label><input type="radio" name="pay"> Платные</label>
            <label><input type="radio" name="pay"> Бесплатные</label>
          </div>
          <button class="btn btn-outline map-btn">На карте 📍</button>
        </div>

        <!-- Секция 1: Силовой спорт -->
        <h2 class="section-title">Силовой спорт</h2>
        
        <div class="cards-list">
          <!-- Карточка 1 -->
          <div class="card">
            <div class="card-img">
              <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
            </div>
            <div class="card-info">
              <div class="card-header">
                <div>
                  <h3 class="card-title">Тяжелая атлетика<br><span>(в Юбилейном мкр.)</span></h3>
                  <p class="card-hashtag">#Тяжелая атлетика</p>
                </div>
                <span class="badge badge-red">Бесплатно</span>
              </div>
              <div class="card-details">
                <p><span class="icon">👤</span> 10-18 лет</p>
                <p><span class="icon">📍</span> г. Иркутск, Юбилейный мкр, стр. 49/1</p>
                <p><span class="icon">🏢</span> ФОК "Юбилейный"</p>
              </div>
              <div class="card-footer">
                <div class="schedule">
                  <span class="days">Пн, Ср, Пт</span>
                  <div class="time-tags">
                    <span class="time-tag">09:00 - 10:30</span>
                    <span class="time-tag">12:00 - 13:30</span>
                    <span class="time-tag">18:00 - 19:30</span>
                  </div>
                </div>
                <router-link to="/detail" class="btn btn-primary">Подробнее</router-link>
              </div>
            </div>
          </div>

          <!-- Карточка 2 -->
          <div class="card">
            <div class="card-img">
              <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
            </div>
            <div class="card-info">
              <div class="card-header">
                <div>
                  <h3 class="card-title">Тяжелая атлетика<br><span>(на ул. Боткина)</span></h3>
                  <p class="card-hashtag">#Тяжелая атлетика</p>
                </div>
                <div class="badges-group">
                  <span class="badge badge-outline">Первое бесплатно</span>
                  <span class="badge badge-red">300 руб.</span>
                </div>
              </div>
              <div class="card-details">
                <p><span class="icon">👤</span> 10-18 лет</p>
                <p><span class="icon">📍</span> г. Иркутск, Юбилейный мкр, стр. 49/1</p>
                <p><span class="icon">🏢</span> ФОК "Юбилейный"</p>
              </div>
              <div class="card-footer">
                <div class="schedule">
                  <span class="days">Пн, Ср, Пт</span>
                  <div class="time-tags">
                    <span class="time-tag">09:00 - 10:30</span>
                    <span class="time-tag">12:00 - 13:30</span>
                  </div>
                </div>
                <router-link to="/detail" class="btn btn-primary">Подробнее</router-link>
              </div>
            </div>
          </div>
        </div>

        <!-- Секция 2: Единоборства -->
        <h2 class="section-title mt-30">Единоборства</h2>
        
        <div class="cards-list">
          <!-- Карточка 3 -->
          <div class="card">
            <div class="card-img">
              <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
            </div>
            <div class="card-info">
              <div class="card-header">
                <div>
                  <h3 class="card-title">Дзюдо</h3>
                  <p class="card-hashtag">#Дзюдо</p>
                </div>
                <span class="badge badge-red">Бесплатно</span>
              </div>
              <div class="card-details">
                <p><span class="icon">👤</span> 6-18 лет</p>
                <p><span class="icon">📍</span> г. Иркутск, ул. Трудовая, д. 115А</p>
                <p><span class="icon">🏢</span> СК "Вымпел"</p>
              </div>
              <div class="card-footer">
                <div class="schedule">
                  <span class="days">Пн, Ср, Пт</span>
                  <div class="time-tags">
                    <span class="time-tag">09:00 - 10:30</span>
                    <span class="time-tag">12:00 - 13:30</span>
                    <span class="time-tag">18:00 - 19:30</span>
                  </div>
                </div>
                <router-link to="/detail" class="btn btn-primary">Подробнее</router-link>
              </div>
            </div>
          </div>

          <!-- Карточка 4 -->
          <div class="card">
            <div class="card-img">
              <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2" ry="2"></rect><circle cx="8.5" cy="8.5" r="1.5"></circle><polyline points="21 15 16 10 5 21"></polyline></svg>
            </div>
            <div class="card-info">
              <div class="card-header">
                <div>
                  <h3 class="card-title">Вольная борьба<br><span>(на ул. Норильская)</span></h3>
                  <p class="card-hashtag">#Дзюдо</p>
                </div>
                <div class="badges-group">
                  <span class="badge badge-outline">Первое бесплатно</span>
                  <span class="badge badge-red">300 руб. / месяц</span>
                </div>
              </div>
              <div class="card-details">
                <p><span class="icon">👤</span> 6-18 лет</p>
                <p><span class="icon">📍</span> г. Иркутск, ул. Трудовая, д. 115А</p>
                <p><span class="icon">🏢</span> СК "Вымпел"</p>
              </div>
              <div class="card-footer">
                <div class="schedule">
                  <span class="days">Пн, Ср, Пт</span>
                  <div class="time-tags">
                    <span class="time-tag">09:00 - 10:30</span>
                    <span class="time-tag">12:00 - 13:30</span>
                    <span class="time-tag">18:00 - 19:30</span>
                  </div>
                </div>
                <router-link to="/detail" class="btn btn-primary">Подробнее</router-link>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Правая колонка (Фильтры) -->
      <aside class="sidebar">
        <h3 class="sidebar-title">Фильтры</h3>
        
        <div class="filter-block">
          <label>Возраст</label>
          <select class="filter-select"><option>Любой</option></select>
        </div>

        <div class="filter-block">
          <label>Пол</label>
          <div class="checkbox-group">
            <label class="custom-checkbox">
              <input type="checkbox" checked> 
              <span class="checkmark"></span>
              Мужской
            </label>
            <label class="custom-checkbox">
              <input type="checkbox" checked> 
              <span class="checkmark"></span>
              Женский
            </label>
          </div>
        </div>

        <div class="filter-block category-list">
          <label>Каталог</label>
          <ul>
            <li v-for="(cat, index) in categories" :key="index" class="cat-item">
              <div class="cat-header" @click="toggleCategory(cat)">
                <span class="cat-name">{{ cat.name }}</span>
                <span class="count" v-if="cat.count">{{ cat.count }}</span>
                <span class="arrow" :class="{ 'open': cat.isOpen }">
                  <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                    <polyline points="6 9 12 15 18 9"></polyline>
                  </svg>
                </span>
              </div>
              
              <!-- Подкатегории -->
              <ul class="sub-cats" v-show="cat.isOpen && cat.sub">
                <li v-for="(sub, sIndex) in cat.sub" :key="sIndex">
                  <span class="bullet">•</span>
                  <span class="sub-name">{{ sub.name }}</span>
                  <span class="count">{{ sub.count }}</span>
                </li>
              </ul>
            </li>
          </ul>
        </div>
      </aside>
    </div>
  </div>
</template>

<script setup>
import { reactive } from 'vue'
import Header from '../components/Header.vue'

const categories = reactive([
  { name: 'Силовой спорт', count: 3, isOpen: true, sub: [{ name: 'Тяжелая атлетика', count: 3 }, { name: 'Пауэрлифтинг', count: 1 }] },
  { name: 'Единоборства', count: 2, isOpen: true, sub: [{ name: 'Вольная борьба', count: 1 }, { name: 'Дзюдо', count: 1 }] },
  { name: 'ДПИ и ремесла', isOpen: false },
  { name: 'Техническое конструирование', isOpen: false },
  { name: 'Словесность', isOpen: false },
  { name: 'Иностранные языки', isOpen: false },
  { name: 'Развитие интеллекта', isOpen: false },
  { name: 'Информационные технологии', isOpen: false },
  { name: 'История и Традиции', isOpen: false },
  { name: 'Педагогика', isOpen: false },
  { name: 'Музыка и звук', isOpen: false },
  { name: 'Пение', isOpen: false },
  { name: 'Хореография(танцы)', isOpen: false },
  { name: 'Зрелищные искусства', isOpen: false },
  { name: 'Мода и стиль', isOpen: false },
  { name: 'Познавательные развлечения', isOpen: false },
  { name: 'Туризм', isOpen: false },
  { name: 'Естественные науки', isOpen: false },
  { name: 'Люди и животные', isOpen: false },
  { name: 'Эстетические виды спорта', isOpen: false },
  { name: 'Технические виды спорта', isOpen: false },
  { name: 'Командно-игровой спорт', isOpen: false },
  { name: 'Индивидуально игровой спорт', isOpen: false },
  { name: 'Водные виды спорта', isOpen: false },
  { name: 'Лёгкая атлетика и гимнастика', isOpen: false },
  { name: 'Физкультура', isOpen: false }
])

const toggleCategory = (cat) => {
  if (cat.sub) {
    cat.isOpen = !cat.isOpen
  }
}
</script>

<style scoped>
/* --- Общие стили страницы (без изменений) --- */
.layout { display: flex; gap: 24px; margin-top: 20px; align-items: flex-start; }
.main-content { flex: 1; min-width: 0; }
.search-panel { background: white; border-radius: 4px; padding: 10px 16px; display: flex; align-items: center; gap: 20px; margin-bottom: 24px; border: 1px solid var(--border-color); }
.search-input-wrapper { display: flex; align-items: center; gap: 8px; flex: 1; background: #F8F8F8; padding: 8px 12px; border-radius: 4px; border: 1px solid #EEE; }
.search-input-wrapper input { border: none; background: transparent; outline: none; width: 100%; font-size: 13px; }
.search-icon { color: #999; font-size: 14px; }
.radio-group { display: flex; gap: 16px; font-size: 13px; color: #555; }
.map-btn { white-space: nowrap; font-size: 12px; }
.section-title { font-size: 18px; font-weight: 600; margin-bottom: 16px; color: #222; }
.mt-30 { margin-top: 30px; }
.cards-list { display: flex; flex-direction: column; gap: 12px; }
.card { background: white; border-radius: 4px; padding: 16px; display: flex; gap: 20px; border: 1px solid var(--border-color); }
.card-img { width: 140px; height: 140px; background: #C4C4C4; border-radius: 8px; display: flex; align-items: center; justify-content: center; }
.card-info { flex: 1; display: flex; flex-direction: column; }
.card-header { display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 6px; }
.card-title { font-size: 15px; color: #222; font-weight: 600; margin-bottom: 4px; }
.card-title span { font-size: 13px; font-weight: 400; color: #666; }
.card-hashtag { font-size: 12px; color: #999; margin-bottom: 8px; }
.badges-group { display: flex; gap: 8px; }
.card-details p { font-size: 13px; color: #444; margin-bottom: 4px; display: flex; align-items: center; }
.card-details .icon { width: 18px; display: inline-block; color: #666; font-size: 12px; }
.card-footer { display: flex; justify-content: space-between; align-items: flex-end; margin-top: auto; padding-top: 12px; }
.schedule { display: flex; align-items: center; gap: 12px; }
.days { font-size: 13px; color: #444; }
.time-tags { display: flex; gap: 6px; }
.time-tag { background: var(--tag-bg); color: var(--tag-text); padding: 4px 8px; border-radius: 4px; font-size: 11px; font-weight: 500; }

/* --- Стили Сайдбара (Обновленные) --- */
.sidebar {
  width: 300px;
  background: white;
  border-radius: 4px;
  padding: 20px;
  border: 1px solid var(--border-color);
}
.sidebar-title {
  font-size: 18px;
  font-weight: 600;
  margin-bottom: 20px;
  color: #222;
}
.filter-block {
  margin-bottom: 20px;
  border-bottom: 1px solid var(--border-color);
  padding-bottom: 16px;
}
.filter-block > label {
  display: block;
  font-size: 14px;
  font-weight: 500;
  margin-bottom: 10px;
  color: #222;
}
.filter-select {
  width: 100%;
  padding: 8px 10px;
  border: 1px solid var(--border-color);
  border-radius: 4px;
  outline: none;
  font-size: 13px;
  color: #555;
  appearance: none;
  background: url('data:image/svg+xml;utf8,<svg fill="%23666" height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg"><path d="M7 10l5 5 5-5z"/><path d="M0 0h24v24H0z" fill="none"/></svg>') no-repeat right 8px center;
}

/* Кастомные чекбоксы для "Пол" */
.checkbox-group {
  display: flex;
  gap: 16px;
  font-size: 13px;
  color: #444;
}
.custom-checkbox {
  display: flex;
  align-items: center;
  cursor: pointer;
  position: relative;
  user-select: none;
}
.custom-checkbox input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
  height: 0;
  width: 0;
}
.checkmark {
  height: 16px;
  width: 16px;
  background-color: white;
  border: 1px solid #ccc;
  border-radius: 3px;
  margin-right: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
}
.custom-checkbox input:checked ~ .checkmark {
  background-color: var(--primary);
  border-color: var(--primary);
}
.checkmark:after {
  content: "";
  display: none;
  width: 4px;
  height: 8px;
  border: solid white;
  border-width: 0 2px 2px 0;
  transform: rotate(45deg);
}
.custom-checkbox input:checked ~ .checkmark:after {
  display: block;
}

/* Древовидный список категорий */
.category-list ul {
  list-style: none;
  padding: 0;
  margin: 0;
}
.cat-item {
  font-size: 13px;
  padding: 4px 0;
}
.cat-header {
  display: flex;
  align-items: center;
  cursor: pointer;
  padding: 6px 0;
}
.cat-name {
  color: #333;
  flex: 1;
}
.cat-header .count {
  color: #999;
  font-size: 13px;
  margin-right: 12px;
}
.cat-header .arrow {
  color: var(--primary); /* Бордовый цвет стрелочки */
  display: flex;
  align-items: center;
  transition: transform 0.2s ease;
}
.cat-header .arrow.open {
  transform: rotate(180deg); /* Разворачиваем при открытии */
}

/* Подкатегории */
.sub-cats {
  padding-left: 8px !important;
  margin-bottom: 8px !important;
}
.sub-cats li {
  display: flex;
  align-items: center;
  padding: 6px 0;
  color: #555;
}
.sub-cats .bullet {
  color: #999;
  margin-right: 8px;
  font-size: 16px;
  line-height: 1;
}
.sub-cats .sub-name {
  flex: 1;
}
.sub-cats .count {
  color: #999;
  font-size: 13px;
  margin-right: 28px; /* Выравнивание под счетчиком главной категории */
}
</style>