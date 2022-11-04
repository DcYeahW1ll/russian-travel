# Проектная работа 3 Майснера Вильгельма  
## Описание проекта. Функциональность. Используемые технологии.
Проектная работа 3 представляет из себя одностраничный сайт, написанный на HTML и CSS, состоящий из 7 блоков. Каждый блок несет инофрмативный характер о:
 + преищумествах путешествия по России; 
 + красотах нашей Родины; 
 + интересных фактах;
 + полезных ресурсах.

При создании сайта использовалась адаптивно-резиновая вёрстка.

```CSS
.lead {
    display: flex;
    flex-direction: column;
    max-width: 984px;
    align-items: center;
    margin: auto;
    margin-top: 56px;
    margin-bottom: 92px;
}

@media all and (max-width: 1024px) {
    .lead {
      margin-top: 48px;
      max-width: 928px;
    }
}

@media all and (max-width: 768px) {
  .lead {
    margin-bottom: 88px;
    max-width: 768px;
  }
}

@media all and (max-width: 320px) {
  .lead {
    max-width:  320px;
    margin-bottom: 64px;
  }
} ```

```CSS
.lead__image {
  max-width: 100%;
}
```

Так же использовался `grid`.

 ```CSS
 .photo-grid {
  max-width: 1184px;
  min-width: auto;
  margin: 92px auto 92px;
  display: grid;
  grid-template-columns: repeat(4, minmax(min-content, max-content));
  gap: 16px;
}

@media all and (max-width: 1024px) {
  .photo-grid {
  max-width: 928px;
  min-width: auto;
  margin: 92px 48px 92px;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px;
}
}

@media all and (max-width: 768px) {
  .photo-grid {
    max-width: 720px;
    margin: 88px 24px 88px;
    grid-template-columns: repeat(2, 1fr);
    gap: 16px;
  }
} 

@media all and (max-width: 320px) {
  .photo-grid {
    max-width: 288px;
    margin: 64px 16px 64px;
    grid-template-columns: repeat(1, 1fr);
    gap: 12px;
  }
}
```

## Планы по доработке проекта

1. Хотелось бы добавить сайту больше интерактива с использованием `JavaScript`.
2. Помимио основной страницы добавить еще несколько.
