# UI设计风格规范

## 一、设计理念

### 1.1 核心价值观
- **智能化与科技感**：体现AI元素和色彩,营造现代、智能的视觉体验
- **清晰与高效**：界面布局清晰,信息层级分明,操作流程高效
- **专业与可信赖**：采用专业的设计语言,传递可靠的技术能力
- **创新与活力**：通过渐变、动画等元素展现创新活力

### 1.2 设计风格定位
- **主风格**：Soft UI Evolution (改进的新拟态风格)
- **辅助风格**：Glassmorphism (毛玻璃效果)
- **视觉特征**：柔和的阴影、渐变色彩、圆角卡片、现代感图标
- **参考风格**：参考VL提示词平台的设计风格，采用蓝紫色渐变背景，简洁现代的设计语言

## 二、颜色系统

### 2.1 Light模式颜色

#### 主色系
```css
/* 主品牌色 - 蓝紫色系（基于VL提示词平台） */
--primary-50: #E0E7FF;
--primary-100: #C7D2FE;
--primary-200: #A5B4FC;
--primary-300: #818CF8;
--primary-400: #6366F1;
--primary-500: #4F46E5;  /* 主色 - 深蓝紫色 */
--primary-600: #4338CA;
--primary-700: #3730A3;
--primary-800: #312E81;
--primary-900: #1E1B4B;

/* 辅助色 - 紫色系 */
--secondary-50: #F5F3FF;
--secondary-100: #EDE9FE;
--secondary-200: #DDD6FE;
--secondary-300: #C4B5FD;
--secondary-400: #A78BFA;
--secondary-500: #8B5CF6;  /* 辅助色 - 紫色 */
--secondary-600: #7C3AED;
--secondary-700: #6D28D9;
--secondary-800: #5B21B6;
--secondary-900: #4C1D95;
```

#### 辅助色
```css
/* 功能色 */
--success-500: #10B981;
--success-600: #059669;

/* 警告色 */
--warning-500: #F59E0B;
--warning-600: #D97706;

/* 错误色 */
--error-500: #EF4444;
--error-600: #DC2626;

/* 信息色 */
--info-500: #3B82F6;
--info-600: #2563EB;
```

#### 中性色
```css
--gray-50: #F9FAFB;
--gray-100: #F3F4F6;
--gray-200: #E5E7EB;
--gray-300: #D1D5DB;
--gray-400: #9CA3AF;
--gray-500: #6B7280;
--gray-600: #4B5563;
--gray-700: #374151;
--gray-800: #1F2937;
--gray-900: #111827;
```

#### 背景与文本
```css
--bg-primary: #FFFFFF;
--bg-secondary: #F8FAFC;
--bg-tertiary: #F1F5F9;
--bg-hero-gradient: linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%);  /* Hero背景渐变 */
--bg-card: #FFFFFF;
--bg-hover: rgba(79, 70, 229, 0.05);
--bg-active: rgba(79, 70, 229, 0.1);

--text-primary: #1F2937;  /* gray-800 */
--text-secondary: #4B5563;  /* gray-600 */
--text-tertiary: #9CA3AF;  /* gray-400 */
--text-inverse: #FFFFFF;
```

### 2.2 Dark模式颜色

```css
/* 主色系 - Dark模式 */
--primary-50: #1E1B4B;
--primary-100: #312E81;
--primary-200: #3730A3;
--primary-300: #4338CA;
--primary-400: #6366F1;
--primary-500: #818CF8;  /* 主色 - 更亮 */
--primary-600: #A5B4FC;
--primary-700: #C7D2FE;
--primary-800: #E0E7FF;
--primary-900: #F5F3FF;

/* 辅助色 - Dark模式 */
--secondary-500: #A78BFA;  /* 更亮 */
--secondary-600: #C4B5FD;
--secondary-700: #DDD6FE;

/* 背景与文本 - Dark模式 */
--bg-primary: #111827;
--bg-secondary: #1F2937;
--bg-tertiary: #374151;
--bg-hero-gradient: linear-gradient(135deg, #3730A3 0%, #6D28D9 100%);
--bg-card: #1F2937;
--bg-hover: rgba(139, 92, 246, 0.15);
--bg-active: rgba(139, 92, 246, 0.25);

--text-primary: #F9FAFB;
--text-secondary: #D1D5DB;
--text-tertiary: #9CA3AF;
--text-inverse: #111827;
```

### 2.3 渐变色系

```css
/* Hero背景渐变 */
--gradient-hero: linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%);

/* 按钮渐变 */
--gradient-primary: linear-gradient(135deg, #4F46E5 0%, #4338CA 100%);
--gradient-secondary: linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%);

/* AI主题渐变 */
--gradient-ai: linear-gradient(135deg, #4F46E5 0%, #3B82F6 100%);

/* 功能渐变 */
--gradient-success: linear-gradient(135deg, #10B981 0%, #34D399 100%);
--gradient-warning: linear-gradient(135deg, #F59E0B 0%, #FBBF24 100%);
--gradient-error: linear-gradient(135deg, #EF4444 0%, #F87171 100%);
```

### 2.4 透明度系统

```css
/* 玻璃效果透明度 */
--glass-light: rgba(255, 255, 255, 0.8);
--glass-medium: rgba(255, 255, 255, 0.6);
--glass-dark: rgba(255, 255, 255, 0.4);

/* Dark模式玻璃效果 */
--glass-dark-light: rgba(17, 24, 39, 0.8);
--glass-dark-medium: rgba(17, 24, 39, 0.6);
--glass-dark-dark: rgba(17, 24, 39, 0.4);

/* 卡片透明度 */
--card-overlay-light: rgba(255, 255, 255, 0.9);
--card-overlay-dark: rgba(31, 41, 55, 0.9);
```

### 2.5 阴影系统

```css
/* Soft UI Evolution 阴影 */
--shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
--shadow-2xl: 0 25px 50px -12px rgba(0, 0, 0, 0.25);

/* 彩色阴影 - AI主题 */
--shadow-primary: 0 4px 14px 0 rgba(79, 70, 229, 0.39);
--shadow-secondary: 0 4px 14px 0 rgba(139, 92, 246, 0.39);
--shadow-ai: 0 4px 14px 0 rgba(59, 130, 246, 0.39);
```

### 2.6 Tailwind配置示例

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: {
          50: '#E0E7FF',
          100: '#C7D2FE',
          200: '#A5B4FC',
          300: '#818CF8',
          400: '#6366F1',
          500: '#4F46E5',
          600: '#4338CA',
          700: '#3730A3',
          800: '#312E81',
          900: '#1E1B4B',
        },
        secondary: {
          50: '#F5F3FF',
          100: '#EDE9FE',
          200: '#DDD6FE',
          300: '#C4B5FD',
          400: '#A78BFA',
          500: '#8B5CF6',
          600: '#7C3AED',
          700: '#6D28D9',
          800: '#5B21B6',
          900: '#4C1D95',
        },
      },
      backgroundImage: {
        'hero-gradient': 'linear-gradient(135deg, #4F46E5 0%, #7C3AED 100%)',
        'gradient-primary': 'linear-gradient(135deg, #4F46E5 0%, #4338CA 100%)',
        'gradient-secondary': 'linear-gradient(135deg, #8B5CF6 0%, #7C3AED 100%)',
        'gradient-ai': 'linear-gradient(135deg, #4F46E5 0%, #3B82F6 100%)',
      },
    },
  },
}
```

## 三、字体系统

### 3.1 字体选择

#### 中文字体
```css
/* 字体家族 */
--font-family-heading: 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', sans-serif;
--font-family-body: 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', sans-serif;

/* 备选字体 - 现代无衬线 */
--font-family-modern: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

#### 英文字体 (可选,用于国际化)
```css
/* Google Fonts 导入 */
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap');

--font-family-heading-en: 'Plus Jakarta Sans', sans-serif;
--font-family-body-en: 'Plus Jakarta Sans', sans-serif;
```

### 3.2 字号层级

```css
/* 超大标题 */
--text-5xl: 3rem;     /* 48px - 页面主标题 */
--text-4xl: 2.25rem;  /* 36px - 区块标题 */

/* 大标题 */
--text-3xl: 1.875rem; /* 30px - 子页面标题 */

/* 中等标题 */
--text-2xl: 1.5rem;   /* 24px - 卡片标题、区块标题 */
--text-xl: 1.25rem;   /* 20px - 小节标题 */

/* 正文 */
--text-lg: 1.125rem;  /* 18px - 重要正文 */
--text-base: 1rem;    /* 16px - 标准正文 */
--text-sm: 0.875rem;  /* 14px - 辅助文本 */
--text-xs: 0.75rem;   /* 12px - 标签、提示文本 */
--text-2xs: 0.625rem; /* 10px - 最小文本 */
```

### 3.3 字重层级

```css
--font-weight-thin: 100;
--font-weight-light: 300;
--font-weight-normal: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--font-weight-extrabold: 800;
```

### 3.4 行高规范

```css
--leading-tight: 1.25;   /* 标题 */
--leading-normal: 1.5;   /* 正文 */
--leading-relaxed: 1.75; /* 长文本 */
--leading-loose: 2;      /* 特殊场景 */
```

### 3.5 字母间距

```css
--tracking-tighter: -0.05em;  /* 紧凑 */
--tracking-tight: -0.025em;   /* 较紧凑 */
--tracking-normal: 0;         /* 正常 */
--tracking-wide: 0.025em;     /* 较宽 */
--tracking-wider: 0.05em;     /* 宽 */
```

### 3.6 字体使用规范

| 文本类型 | 字号 | 字重 | 行高 | 使用场景 |
|---------|------|------|------|---------|
| 页面主标题 | 48px (text-5xl) | 700 (bold) | 1.25 | 首页Hero、主要标题 |
| 区块标题 | 36px (text-4xl) | 700 (bold) | 1.25 | 大区块标题 |
| 子页面标题 | 30px (text-3xl) | 600 (semibold) | 1.25 | 页面标题 |
| 卡片标题 | 24px (text-2xl) | 600 (semibold) | 1.25 | 卡片标题 |
| 小节标题 | 20px (text-xl) | 600 (semibold) | 1.5 | 内容区块标题 |
| 重要正文 | 18px (text-lg) | 500 (medium) | 1.5 | 重点说明 |
| 标准正文 | 16px (text-base) | 400 (normal) | 1.5 | 常规文本 |
| 辅助文本 | 14px (text-sm) | 400 (normal) | 1.5 | 次要信息 |
| 标签文本 | 12px (text-xs) | 500 (medium) | 1.5 | 标签、徽章 |
| 最小文本 | 10px (text-2xs) | 400 (normal) | 1.5 | 提示信息 |

### 3.7 Tailwind配置示例

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      fontFamily: {
        sans: ['PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'sans-serif'],
        heading: ['PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'sans-serif'],
      },
      fontSize: {
        '5xl': ['3rem', { lineHeight: '1.25', fontWeight: '700' }],
        '4xl': ['2.25rem', { lineHeight: '1.25', fontWeight: '700' }],
        '3xl': ['1.875rem', { lineHeight: '1.25', fontWeight: '600' }],
        '2xl': ['1.5rem', { lineHeight: '1.25', fontWeight: '600' }],
        'xl': ['1.25rem', { lineHeight: '1.5', fontWeight: '600' }],
        'lg': ['1.125rem', { lineHeight: '1.5', fontWeight: '500' }],
        'base': ['1rem', { lineHeight: '1.5', fontWeight: '400' }],
        'sm': ['0.875rem', { lineHeight: '1.5', fontWeight: '400' }],
        'xs': ['0.75rem', { lineHeight: '1.5', fontWeight: '500' }],
      },
    },
  },
}
```

## 二、颜色系统

### 2.1 Light模式颜色

#### 主色系
```css
/* 主品牌色 - AI紫色系 */
--primary-50: #FAF5FF;
--primary-100: #F3E8FF;
--primary-200: #E9D5FF;
--primary-300: #D8B4FE;
--primary-400: #C084FC;
--primary-500: #A855F7;  /* 主色 */
--primary-600: #9333EA;
--primary-700: #7E22CE;
--primary-800: #6B21A8;
--primary-900: #581C87;
```

#### 辅助色
```css
/* 辅助色 - 青色系 */
--secondary-50: #ECFEFF;
--secondary-100: #CFFAFE;
--secondary-200: #A5F3FC;
--secondary-300: #67E8F9;
--secondary-400: #22D3EE;
--secondary-500: #06B6D4;  /* 辅助色 */
--secondary-600: #0891B2;
--secondary-700: #0E7490;
--secondary-800: #155E75;
--secondary-900: #164E63;
```

#### 功能色
```css
/* 成功色 */
--success-500: #10B981;
--success-600: #059669;

/* 警告色 */
--warning-500: #F59E0B;
--warning-600: #D97706;

/* 错误色 */
--error-500: #EF4444;
--error-600: #DC2626;

/* 信息色 */
--info-500: #3B82F6;
--info-600: #2563EB;
```

#### 中性色
```css
--gray-50: #F9FAFB;
--gray-100: #F3F4F6;
--gray-200: #E5E7EB;
--gray-300: #D1D5DB;
--gray-400: #9CA3AF;
--gray-500: #6B7280;
--gray-600: #4B5563;
--gray-700: #374151;
--gray-800: #1F2937;
--gray-900: #111827;
```

#### 背景与文本
```css
--bg-primary: #FFFFFF;
--bg-secondary: #FAF5FF;
--bg-tertiary: #F3E8FF;
--bg-hover: rgba(168, 85, 247, 0.05);
--bg-active: rgba(168, 85, 247, 0.1);

--text-primary: #1F2937;  /* gray-800 */
--text-secondary: #4B5563;  /* gray-600 */
--text-tertiary: #9CA3AF;  /* gray-400 */
--text-inverse: #FFFFFF;
```

### 2.2 Dark模式颜色

```css
/* 主色系 - Dark模式 */
--primary-50: #581C87;
--primary-100: #6B21A8;
--primary-200: #7E22CE;
--primary-300: #9333EA;
--primary-400: #A855F7;
--primary-500: #C084FC;  /* 主色 - 更亮 */
--primary-600: #D8B4FE;
--primary-700: #E9D5FF;
--primary-800: #F3E8FF;
--primary-900: #FAF5FF;

/* 辅助色 - Dark模式 */
--secondary-500: #22D3EE;  /* 更亮 */
--secondary-600: #67E8F9;
--secondary-700: #A5F3FC;

/* 背景与文本 - Dark模式 */
--bg-primary: #111827;
--bg-secondary: #1F2937;
--bg-tertiary: #374151;
--bg-hover: rgba(168, 85, 247, 0.15);
--bg-active: rgba(168, 85, 247, 0.25);

--text-primary: #F9FAFB;
--text-secondary: #D1D5DB;
--text-tertiary: #9CA3AF;
--text-inverse: #111827;
```

### 2.3 渐变色系

```css
/* AI主题渐变 */
--gradient-primary: linear-gradient(135deg, #A855F7 0%, #06B6D4 100%);
--gradient-secondary: linear-gradient(135deg, #7E22CE 0%, #0891B2 100%);
--gradient-soft: linear-gradient(135deg, rgba(168, 85, 247, 0.1) 0%, rgba(6, 182, 212, 0.1) 100%);

/* 功能渐变 */
--gradient-success: linear-gradient(135deg, #10B981 0%, #34D399 100%);
--gradient-warning: linear-gradient(135deg, #F59E0B 0%, #FBBF24 100%);
--gradient-error: linear-gradient(135deg, #EF4444 0%, #F87171 100%);
```

### 2.4 透明度系统

```css
/* 玻璃效果透明度 */
--glass-light: rgba(255, 255, 255, 0.8);
--glass-medium: rgba(255, 255, 255, 0.6);
--glass-dark: rgba(255, 255, 255, 0.4);

/* Dark模式玻璃效果 */
--glass-dark-light: rgba(17, 24, 39, 0.8);
--glass-dark-medium: rgba(17, 24, 39, 0.6);
--glass-dark-dark: rgba(17, 24, 39, 0.4);
```

### 2.5 阴影系统

```css
/* Soft UI Evolution 阴影 */
--shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
--shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
--shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
--shadow-xl: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
--shadow-2xl: 0 25px 50px -12px rgba(0, 0, 0, 0.25);

/* 彩色阴影 - AI主题 */
--shadow-primary: 0 4px 14px 0 rgba(168, 85, 247, 0.39);
--shadow-secondary: 0 4px 14px 0 rgba(6, 182, 212, 0.39);
```

### 2.6 Tailwind配置示例

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: {
          50: '#FAF5FF',
          100: '#F3E8FF',
          200: '#E9D5FF',
          300: '#D8B4FE',
          400: '#C084FC',
          500: '#A855F7',
          600: '#9333EA',
          700: '#7E22CE',
          800: '#6B21A8',
          900: '#581C87',
        },
        secondary: {
          50: '#ECFEFF',
          100: '#CFFAFE',
          200: '#A5F3FC',
          300: '#67E8F9',
          400: '#22D3EE',
          500: '#06B6D4',
          600: '#0891B2',
          700: '#0E7490',
          800: '#155E75',
          900: '#164E63',
        },
      },
      backgroundImage: {
        'gradient-primary': 'linear-gradient(135deg, #A855F7 0%, #06B6D4 100%)',
        'gradient-secondary': 'linear-gradient(135deg, #7E22CE 0%, #0891B2 100%)',
      },
    },
  },
}
```

## 三、字体系统

### 3.1 字体选择

#### 中文字体
```css
/* 字体家族 */
--font-family-heading: 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', sans-serif;
--font-family-body: 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', sans-serif;

/* 备选字体 - 现代无衬线 */
--font-family-modern: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
```

#### 英文字体 (可选,用于国际化)
```css
/* Google Fonts 导入 */
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap');

--font-family-heading-en: 'Plus Jakarta Sans', sans-serif;
--font-family-body-en: 'Plus Jakarta Sans', sans-serif;
```

### 3.2 字号层级

```css
/* 超大标题 */
--text-5xl: 3rem;     /* 48px - 页面主标题 */
--text-4xl: 2.25rem;  /* 36px - 区块标题 */

/* 大标题 */
--text-3xl: 1.875rem; /* 30px - 子页面标题 */

/* 中等标题 */
--text-2xl: 1.5rem;   /* 24px - 卡片标题、区块标题 */
--text-xl: 1.25rem;   /* 20px - 小节标题 */

/* 正文 */
--text-lg: 1.125rem;  /* 18px - 重要正文 */
--text-base: 1rem;    /* 16px - 标准正文 */
--text-sm: 0.875rem;  /* 14px - 辅助文本 */
--text-xs: 0.75rem;   /* 12px - 标签、提示文本 */
--text-2xs: 0.625rem; /* 10px - 最小文本 */
```

### 3.3 字重层级

```css
--font-weight-thin: 100;
--font-weight-light: 300;
--font-weight-normal: 400;
--font-weight-medium: 500;
--font-weight-semibold: 600;
--font-weight-bold: 700;
--font-weight-extrabold: 800;
```

### 3.4 行高规范

```css
--leading-tight: 1.25;   /* 标题 */
--leading-normal: 1.5;   /* 正文 */
--leading-relaxed: 1.75; /* 长文本 */
--leading-loose: 2;      /* 特殊场景 */
```

### 3.5 字母间距

```css
--tracking-tighter: -0.05em;  /* 紧凑 */
--tracking-tight: -0.025em;   /* 较紧凑 */
--tracking-normal: 0;         /* 正常 */
--tracking-wide: 0.025em;     /* 较宽 */
--tracking-wider: 0.05em;     /* 宽 */
```

### 3.6 字体使用规范

| 文本类型 | 字号 | 字重 | 行高 | 使用场景 |
|---------|------|------|------|---------|
| 页面主标题 | 48px (text-5xl) | 700 (bold) | 1.25 | 首页Hero、主要标题 |
| 区块标题 | 36px (text-4xl) | 700 (bold) | 1.25 | 大区块标题 |
| 子页面标题 | 30px (text-3xl) | 600 (semibold) | 1.25 | 页面标题 |
| 卡片标题 | 24px (text-2xl) | 600 (semibold) | 1.25 | 卡片标题 |
| 小节标题 | 20px (text-xl) | 600 (semibold) | 1.5 | 内容区块标题 |
| 重要正文 | 18px (text-lg) | 500 (medium) | 1.5 | 重点说明 |
| 标准正文 | 16px (text-base) | 400 (normal) | 1.5 | 常规文本 |
| 辅助文本 | 14px (text-sm) | 400 (normal) | 1.5 | 次要信息 |
| 标签文本 | 12px (text-xs) | 500 (medium) | 1.5 | 标签、徽章 |
| 最小文本 | 10px (text-2xs) | 400 (normal) | 1.5 | 提示信息 |

### 3.7 Tailwind配置示例

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      fontFamily: {
        sans: ['PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'sans-serif'],
        heading: ['PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'sans-serif'],
      },
      fontSize: {
        '5xl': ['3rem', { lineHeight: '1.25', fontWeight: '700' }],
        '4xl': ['2.25rem', { lineHeight: '1.25', fontWeight: '700' }],
        '3xl': ['1.875rem', { lineHeight: '1.25', fontWeight: '600' }],
        '2xl': ['1.5rem', { lineHeight: '1.25', fontWeight: '600' }],
        'xl': ['1.25rem', { lineHeight: '1.5', fontWeight: '600' }],
        'lg': ['1.125rem', { lineHeight: '1.5', fontWeight: '500' }],
        'base': ['1rem', { lineHeight: '1.5', fontWeight: '400' }],
        'sm': ['0.875rem', { lineHeight: '1.5', fontWeight: '400' }],
        'xs': ['0.75rem', { lineHeight: '1.5', fontWeight: '500' }],
      },
    },
  },
}
```

## 四、间距系统

### 4.1 基础间距单位

```css
--spacing-0: 0;
--spacing-1: 0.25rem;  /* 4px */
--spacing-2: 0.5rem;   /* 8px */
--spacing-3: 0.75rem;  /* 12px */
--spacing-4: 1rem;     /* 16px - 基础单位 */
--spacing-5: 1.25rem;  /* 20px */
--spacing-6: 1.5rem;   /* 24px */
--spacing-8: 2rem;     /* 32px */
--spacing-10: 2.5rem;  /* 40px */
--spacing-12: 3rem;    /* 48px */
--spacing-16: 4rem;    /* 64px */
--spacing-20: 5rem;    /* 80px */
--spacing-24: 6rem;    /* 96px */
```

### 4.2 组件间距规范

| 组件类型 | 内边距 | 外边距 | 使用场景 |
|---------|--------|--------|---------|
| 按钮(小) | px-3 py-1.5 | - | 小型按钮 |
| 按钮(中) | px-4 py-2 | - | 标准按钮 |
| 按钮(大) | px-6 py-3 | - | 大型按钮、CTA按钮 |
| 输入框 | px-4 py-2.5 | mb-4 | 表单输入 |
| 卡片 | p-6 | mb-6 | 标准卡片 |
| 模态框 | p-6 | - | 弹窗内容 |
| 导航项 | px-4 py-3 | - | 导航菜单 |
| 标签 | px-2.5 py-1 | mr-2 | 标签徽章 |
| 头像容器 | - | mr-3 | 用户头像 |

### 4.3 页面布局间距

| 布局元素 | 间距值 | 说明 |
|---------|--------|------|
| 页面外边距 | px-6 py-8 | 标准页面内外边距 |
| 页面最大宽度 | max-w-7xl (1280px) | 内容容器最大宽度 |
| 区块间距 | space-y-8 | 垂直区块间距 |
| 卡片间距 | grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 | 卡片网格间距 |
| 表单项间距 | mb-4 | 表单元素间距 |
| 列表项间距 | mb-4 | 列表元素间距 |

### 4.4 间距使用原则

1. **一致性**：同类组件使用相同间距
2. **节奏感**：保持8px倍数的间距体系
3. **呼吸感**：重要内容周围留有足够空白
4. **对齐**：元素对齐遵循网格系统
5. **响应式**：移动端适当减小间距

## 五、布局栅格系统

### 5.1 断点系统

```css
/* 断点定义 */
--breakpoint-sm: 640px;   /* 手机横屏/小平板 */
--breakpoint-md: 768px;   /* 平板竖屏 */
--breakpoint-lg: 1024px;  /* 平板横屏/小笔记本 */
--breakpoint-xl: 1280px;  /* 标准桌面 */
--breakpoint-2xl: 1536px; /* 大屏桌面 */
```

### 5.2 容器系统

```css
/* 容器宽度 */
--container-sm: 640px;
--container-md: 768px;
--container-lg: 1024px;
--container-xl: 1280px;
--container-2xl: 1536px;
```

### 5.3 栅格系统

```css
/* 12列栅格系统 */
--grid-cols-1: repeat(1, 1fr);
--grid-cols-2: repeat(2, 1fr);
--grid-cols-3: repeat(3, 1fr);
--grid-cols-4: repeat(4, 1fr);
--grid-cols-6: repeat(6, 1fr);
--grid-cols-12: repeat(12, 1fr);
```

### 5.4 常用栅格布局

#### 卡片网格
```css
/* 响应式卡片网格 */
.card-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.5rem;
}

@media (min-width: 768px) {
  .card-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1024px) {
  .card-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

#### 标准布局
```css
/* 左侧导航 + 右侧内容 */
.layout-sidebar {
  display: grid;
  grid-template-columns: 1fr;
}

@media (min-width: 1024px) {
  .layout-sidebar {
    grid-template-columns: 280px 1fr;
  }
}

/* 顶部导航 + 主内容 */
.layout-topnav {
  display: flex;
  flex-direction: column;
}

@media (min-width: 768px) {
  .layout-topnav {
    flex-direction: row;
  }
}
```

### 5.5 响应式布局策略

#### 移动优先
```css
/* 默认移动端样式 */
.container {
  padding: 1rem;
}

.content {
  grid-template-columns: 1fr;
}

/* 平板及以上 */
@media (min-width: 768px) {
  .container {
    padding: 2rem;
  }

  .content {
    grid-template-columns: repeat(2, 1fr);
  }
}

/* 桌面及以上 */
@media (min-width: 1024px) {
  .container {
    padding: 3rem;
  }

  .content {
    grid-template-columns: repeat(3, 1fr);
  }
}
```

### 5.6 Tailwind配置示例

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    screens: {
      'sm': '640px',
      'md': '768px',
      'lg': '1024px',
      'xl': '1280px',
      '2xl': '1536px',
    },
    maxWidth: {
      'container': '1280px',
    },
  },
}
```

## 六、组件规范

### 6.1 按钮

**重要说明**: 除 Hero 区域的特殊设计需求外,其他页面的按钮应保持 Tailwind 默认风格,使用 Tailwind 的标准工具类(如 `bg-indigo-600`, `hover:bg-indigo-700`, `bg-gray-200` 等),不使用自定义 CSS 类或全局样式覆盖。

#### Hero区域特殊按钮样式

Hero区域可使用以下自定义样式,仅限该区域使用:
```css
/* 主要按钮 */
.btn-primary {
  background: linear-gradient(135deg, #A855F7 0%, #9333EA 100%);
  color: #FFFFFF;
  padding: 0.75rem 1.5rem;
  border-radius: 0.5rem;
  font-weight: 500;
  transition: all 0.2s ease;
  cursor: pointer;
}

.btn-primary:hover {
  background: linear-gradient(135deg, #9333EA 0%, #7E22CE 100%);
  transform: translateY(-1px);
  box-shadow: 0 4px 12px rgba(168, 85, 247, 0.4);
}

.btn-primary:active {
  transform: translateY(0);
}

/* 次要按钮 */
.btn-secondary {
  background: #FFFFFF;
  color: #A855F7;
  border: 1px solid #A855F7;
  padding: 0.75rem 1.5rem;
  border-radius: 0.5rem;
  font-weight: 500;
  transition: all 0.2s ease;
  cursor: pointer;
}

.btn-secondary:hover {
  background: #FAF5FF;
  border-color: #9333EA;
}

/* 幽灵按钮 */
.btn-ghost {
  background: transparent;
  color: #4B5563;
  padding: 0.75rem 1.5rem;
  border-radius: 0.5rem;
  font-weight: 500;
  transition: all 0.2s ease;
  cursor: pointer;
}

.btn-ghost:hover {
  background: rgba(168, 85, 247, 0.1);
  color: #A855F7;
}

/* 文字按钮 */
.btn-text {
  background: transparent;
  color: #A855F7;
  padding: 0.5rem 1rem;
  font-weight: 500;
  transition: all 0.2s ease;
  cursor: pointer;
}

.btn-text:hover {
  color: #9333EA;
  text-decoration: underline;
}
```

#### 按钮尺寸
```css
/* 小型按钮 */
.btn-sm {
  padding: 0.5rem 1rem;
  font-size: 0.875rem;
}

/* 标准按钮 */
.btn-md {
  padding: 0.75rem 1.5rem;
  font-size: 1rem;
}

/* 大型按钮 */
.btn-lg {
  padding: 1rem 2rem;
  font-size: 1.125rem;
}
```

#### 按钮状态
```css
/* 禁用状态 */
.btn-disabled {
  opacity: 0.5;
  cursor: not-allowed;
  pointer-events: none;
}

/* 加载状态 */
.btn-loading {
  position: relative;
  pointer-events: none;
}

.btn-loading::after {
  content: '';
  position: absolute;
  width: 1rem;
  height: 1rem;
  border: 2px solid rgba(255, 255, 255, 0.3);
  border-top-color: #FFFFFF;
  border-radius: 50%;
  animation: spin 0.6s linear infinite;
}

@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}
```

### 6.2 卡片

#### 基础卡片
```css
.card {
  background: var(--bg-primary);
  border-radius: 0.75rem;
  padding: 1.5rem;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
  transition: all 0.3s ease;
  border: 1px solid var(--gray-200);
}

.card:hover {
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
  transform: translateY(-2px);
}
```

#### 卡片变体
```css
/* 可交互卡片 */
.card-interactive {
  cursor: pointer;
}

.card-interactive:hover {
  border-color: #A855F7;
  box-shadow: 0 10px 15px -3px rgba(168, 85, 247, 0.2);
}

/* 玻璃卡片 */
.card-glass {
  background: rgba(255, 255, 255, 0.7);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.3);
}

/* Dark模式玻璃卡片 */
.dark .card-glass {
  background: rgba(17, 24, 39, 0.7);
  border: 1px solid rgba(255, 255, 255, 0.1);
}
```

### 6.3 输入框

#### 文本输入
```css
.input {
  width: 100%;
  padding: 0.75rem 1rem;
  border: 1px solid var(--gray-300);
  border-radius: 0.5rem;
  font-size: 1rem;
  background: var(--bg-primary);
  color: var(--text-primary);
  transition: all 0.2s ease;
}

.input:focus {
  outline: none;
  border-color: #A855F7;
  box-shadow: 0 0 0 3px rgba(168, 85, 247, 0.1);
}

.input::placeholder {
  color: var(--text-tertiary);
}

.input-error {
  border-color: #EF4444;
}

.input-error:focus {
  box-shadow: 0 0 0 3px rgba(239, 68, 68, 0.1);
}
```

#### 文本域
```css
.textarea {
  width: 100%;
  padding: 0.75rem 1rem;
  border: 1px solid var(--gray-300);
  border-radius: 0.5rem;
  font-size: 1rem;
  background: var(--bg-primary);
  color: var(--text-primary);
  transition: all 0.2s ease;
  resize: vertical;
  min-height: 120px;
}

.textarea:focus {
  outline: none;
  border-color: #A855F7;
  box-shadow: 0 0 0 3px rgba(168, 85, 247, 0.1);
}
```

### 6.4 标签

```css
.tag {
  display: inline-flex;
  align-items: center;
  padding: 0.25rem 0.75rem;
  border-radius: 9999px;
  font-size: 0.75rem;
  font-weight: 500;
}

.tag-primary {
  background: rgba(168, 85, 247, 0.1);
  color: #9333EA;
}

.tag-secondary {
  background: rgba(6, 182, 212, 0.1);
  color: #0891B2;
}

.tag-success {
  background: rgba(16, 185, 129, 0.1);
  color: #059669;
}

.tag-warning {
  background: rgba(245, 158, 11, 0.1);
  color: #D97706;
}

.tag-error {
  background: rgba(239, 68, 68, 0.1);
  color: #DC2626;
}
```

### 6.5 头像

```css
.avatar {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  object-fit: cover;
  border: 2px solid var(--gray-200);
}

.avatar-lg {
  width: 64px;
  height: 64px;
}

.avatar-sm {
  width: 32px;
  height: 32px;
}

.avatar-xs {
  width: 24px;
  height: 24px;
}
```

### 6.6 导航

#### 顶部导航
```css
.navbar {
  position: sticky;
  top: 0;
  z-index: 50;
  background: rgba(255, 255, 255, 0.8);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--gray-200);
}

.dark .navbar {
  background: rgba(17, 24, 39, 0.8);
  border-bottom-color: rgba(255, 255, 255, 0.1);
}

.nav-item {
  display: flex;
  align-items: center;
  padding: 0.75rem 1rem;
  color: var(--text-secondary);
  transition: all 0.2s ease;
  border-radius: 0.5rem;
  cursor: pointer;
}

.nav-item:hover {
  color: var(--text-primary);
  background: rgba(168, 85, 247, 0.1);
}

.nav-item.active {
  color: #A855F7;
  background: rgba(168, 85, 247, 0.1);
}
```

#### 侧边导航
```css
.sidebar {
  position: fixed;
  left: 0;
  top: 0;
  bottom: 0;
  width: 280px;
  background: var(--bg-secondary);
  border-right: 1px solid var(--gray-200);
  overflow-y: auto;
}

@media (max-width: 1023px) {
  .sidebar {
    transform: translateX(-100%);
    transition: transform 0.3s ease;
  }

  .sidebar.open {
    transform: translateX(0);
  }
}
```

## 七、交互规范

### 7.1 动画时长

```css
/* 微交互 */
--duration-fast: 150ms;

/* 标准交互 */
--duration-normal: 200ms;

/* 慢速交互 */
--duration-slow: 300ms;

/* 页面切换 */
--duration-page: 400ms;
```

### 7.2 缓动函数

```css
/* 线性 */
--ease-linear: linear;

/* 标准缓动 */
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);

/* 弹跳缓动 */
--ease-bounce: cubic-bezier(0.68, -0.55, 0.265, 1.55);

/* 进入动画 */
--ease-enter: cubic-bezier(0, 0, 0.2, 1);

/* 退出动画 */
--ease-exit: cubic-bezier(0.4, 0, 1, 1);
```

### 7.3 交互状态

```css
/* Hover状态 */
.hover-effect {
  transition: all var(--duration-normal) var(--ease-in-out);
}

.hover-effect:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(168, 85, 247, 0.3);
}

/* Active状态 */
.active-effect:active {
  transform: scale(0.98);
}

/* Focus状态 */
.focus-effect:focus {
  outline: none;
  box-shadow: 0 0 0 3px rgba(168, 85, 247, 0.3);
}

/* Disabled状态 */
.disabled-effect {
  opacity: 0.5;
  pointer-events: none;
  cursor: not-allowed;
}
```

### 7.4 加载状态

```css
/* 骨架屏 */
.skeleton {
  background: linear-gradient(
    90deg,
    var(--gray-200) 0%,
    var(--gray-100) 50%,
    var(--gray-200) 100%
  );
  background-size: 200% 100%;
  animation: skeleton-loading 1.5s ease-in-out infinite;
}

@keyframes skeleton-loading {
  0% {
    background-position: 200% 0;
  }
  100% {
    background-position: -200% 0;
  }
}

/* 旋转加载 */
.spinner {
  width: 40px;
  height: 40px;
  border: 3px solid var(--gray-200);
  border-top-color: #A855F7;
  border-radius: 50%;
  animation: spin 0.6s linear infinite;
}

@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}
```

### 7.5 页面切换动画

```css
/* 淡入 */
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.fade-in {
  animation: fadeIn var(--duration-normal) var(--ease-in-out);
}

/* 滑入 */
@keyframes slideIn {
  from {
    transform: translateY(20px);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}

.slide-in {
  animation: slideIn var(--duration-slow) var(--ease-out);
}

/* 缩放 */
@keyframes scaleIn {
  from {
    transform: scale(0.9);
    opacity: 0;
  }
  to {
    transform: scale(1);
    opacity: 1;
  }
}

.scale-in {
  animation: scaleIn var(--duration-slow) var(--ease-out);
}
```

### 7.6 减少动画

```css
/* 尊重用户偏好 */
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

## 八、图标系统

### 8.1 图标选择

- **图标库**：使用 SVG 图标（Heroicons、Lucide Icons）
- **图标尺寸**：基于 24x24 视口
- **图标颜色**：继承文本颜色或使用主题色

### 8.2 图标尺寸

```css
/* Tailwind 图标类 */
.icon-xs { width: 0.75rem; height: 0.75rem; }  /* 12px */
.icon-sm { width: 1rem; height: 1rem; }       /* 16px */
.icon-md { width: 1.25rem; height: 1.25rem; } /* 20px */
.icon-lg { width: 1.5rem; height: 1.5rem; }   /* 24px */
.icon-xl { width: 2rem; height: 2rem; }       /* 32px */
```

### 8.3 图标使用规范

1. **一致性**：同一功能使用相同图标
2. **可访问性**：图标按钮需添加 `aria-label`
3. **颜色适配**：Dark模式下图标颜色需适配
4. **无Emoji**：禁止使用 Emoji 作为图标

### 8.4 示例图标组件

```javascript
// React组件示例
const Icon = ({ name, size = 'lg', className = '' }) => {
  const icons = {
    search: <SearchIcon className={`w-${size} h-${size} ${className}`} />,
    user: <UserIcon className={`w-${size} h-${size} ${className}`} />,
    settings: <SettingsIcon className={`w-${size} h-${size} ${className}`} />,
  }

  return icons[name] || null
}
```

## 九、响应式设计规范

### 9.1 响应式断点

| 断点 | 宽度范围 | 设备类型 | 布局策略 |
|------|---------|---------|---------|
| xs | < 640px | 手机竖屏 | 单列布局 |
| sm | 640px - 767px | 手机横屏 | 单列布局，增大间距 |
| md | 768px - 1023px | 平板竖屏 | 双列布局 |
| lg | 1024px - 1279px | 平板横屏/笔记本 | 三列布局 |
| xl | 1280px - 1535px | 标准桌面 | 三列布局，最大宽度限制 |
| 2xl | > 1536px | 大屏桌面 | 四列布局 |

### 9.2 响应式策略

1. **移动优先**：从最小屏幕开始设计，逐步增强
2. **内容优先**：确保核心内容在所有设备上可访问
3. **触摸友好**：移动端交互元素最小 44x44px
4. **图片优化**：使用响应式图片和懒加载
5. **性能优先**：减少移动端不必要的动画和效果

### 9.3 响应式最佳实践

```css
/* 避免水平滚动 */
body {
  overflow-x: hidden;
}

/* 确保可读性 */
@media (max-width: 640px) {
  html {
    font-size: 14px;
  }
}

/* 表格响应式 */
@media (max-width: 768px) {
  .table-wrapper {
    overflow-x: auto;
  }
}

/* 导航响应式 */
@media (max-width: 1024px) {
  .navbar {
    padding: 1rem;
  }
}
```

## 十、无障碍设计规范

### 10.1 色彩对比度

- **正文文本**：最低 4.5:1
- **大号文本（18pt+）**：最低 3:1
- **图标和图形**：最低 3:1
- **UI组件**：最低 3:1

### 10.2 键盘导航

```css
/* 可见焦点状态 */
:focus-visible {
  outline: 2px solid #A855F7;
  outline-offset: 2px;
}

/* 跳过链接 */
.skip-link {
  position: absolute;
  top: -40px;
  left: 0;
  background: #A855F7;
  color: white;
  padding: 8px;
  text-decoration: none;
}

.skip-link:focus {
  top: 0;
}
```

### 10.3 语义化标签

- 使用正确的 HTML5 语义化标签（`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`）
- 为图片提供描述性 `alt` 文本
- 表单控件使用 `<label>` 标签
- 按钮和链接有明确的文本描述

### 10.4 ARIA 属性

```html
<!-- 图标按钮 -->
<button aria-label="搜索">
  <svg>...</svg>
</button>

<!-- 模态框 -->
<div role="dialog" aria-labelledby="modal-title" aria-modal="true">
  <h2 id="modal-title">标题</h2>
</div>

<!-- 加载状态 -->
<div aria-live="polite" aria-busy="true">
  加载中...
</div>
```

## 十一、Tailwind CSS 完整配置

```javascript
// tailwind.config.js
module.exports = {
  darkMode: 'class',
  content: [
    './src/**/*.{js,jsx,ts,tsx}',
    './public/index.html',
  ],
  theme: {
    extend: {
      colors: {
        primary: {
          50: '#FAF5FF',
          100: '#F3E8FF',
          200: '#E9D5FF',
          300: '#D8B4FE',
          400: '#C084FC',
          500: '#A855F7',
          600: '#9333EA',
          700: '#7E22CE',
          800: '#6B21A8',
          900: '#581C87',
        },
        secondary: {
          50: '#ECFEFF',
          100: '#CFFAFE',
          200: '#A5F3FC',
          300: '#67E8F9',
          400: '#22D3EE',
          500: '#06B6D4',
          600: '#0891B2',
          700: '#0E7490',
          800: '#155E75',
          900: '#164E63',
        },
      },
      fontFamily: {
        sans: ['PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'sans-serif'],
        heading: ['PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'sans-serif'],
      },
      fontSize: {
        '5xl': ['3rem', { lineHeight: '1.25', fontWeight: '700' }],
        '4xl': ['2.25rem', { lineHeight: '1.25', fontWeight: '700' }],
        '3xl': ['1.875rem', { lineHeight: '1.25', fontWeight: '600' }],
        '2xl': ['1.5rem', { lineHeight: '1.25', fontWeight: '600' }],
        'xl': ['1.25rem', { lineHeight: '1.5', fontWeight: '600' }],
        'lg': ['1.125rem', { lineHeight: '1.5', fontWeight: '500' }],
        'base': ['1rem', { lineHeight: '1.5', fontWeight: '400' }],
        'sm': ['0.875rem', { lineHeight: '1.5', fontWeight: '400' }],
        'xs': ['0.75rem', { lineHeight: '1.5', fontWeight: '500' }],
      },
      boxShadow: {
        'primary': '0 4px 14px 0 rgba(168, 85, 247, 0.39)',
        'secondary': '0 4px 14px 0 rgba(6, 182, 212, 0.39)',
      },
      backgroundImage: {
        'gradient-primary': 'linear-gradient(135deg, #A855F7 0%, #06B6D4 100%)',
        'gradient-secondary': 'linear-gradient(135deg, #7E22CE 0%, #0891B2 100%)',
      },
      animation: {
        'fade-in': 'fadeIn 0.2s ease-in-out',
        'slide-in': 'slideIn 0.3s ease-out',
        'scale-in': 'scaleIn 0.3s ease-out',
      },
      keyframes: {
        fadeIn: {
          '0%': { opacity: '0' },
          '100%': { opacity: '1' },
        },
        slideIn: {
          '0%': { transform: 'translateY(20px)', opacity: '0' },
          '100%': { transform: 'translateY(0)', opacity: '1' },
        },
        scaleIn: {
          '0%': { transform: 'scale(0.9)', opacity: '0' },
          '100%': { transform: 'scale(1)', opacity: '1' },
        },
      },
    },
  },
  plugins: [
    require('@tailwindcss/forms'),
  ],
}
```

## 十二、设计检查清单

### 12.1 视觉质量
- [ ] 颜色对比度符合 WCAG AA 标准（正文文本 4.5:1+）
- [ ] 字号层级清晰，符合使用规范
- [ ] 间距遵循 8px 基准网格
- [ ] 圆角使用一致（标准：0.5rem - 0.75rem）
- [ ] 阴影效果适度，不影响可读性
- [ ] 图标风格统一，不使用 Emoji

### 12.2 交互体验
- [ ] 所有可点击元素有明确的 hover 状态
- [ ] 按钮点击有反馈（scale、color变化）
- [ ] 动画时长合理（150-300ms）
- [ ] 加载状态清晰（骨架屏、spinner）
- [ ] 错误提示明确且位置合理
- [ ] Focus 状态可见，支持键盘导航

### 12.3 响应式设计
- [ ] 在 375px、768px、1024px、1440px 下测试
- [ ] 移动端无横向滚动
- [ ] 触摸目标最小 44x44px
- [ ] 图片自适应并优化
- [ ] 表格在小屏下可横向滚动

### 12.4 主题切换
- [ ] Light 和 Dark 模式颜色完整
- [ ] 两种模式下对比度都符合标准
- [ ] 过渡动画平滑
- [ ] 主题状态持久化

### 12.5 无障碍设计
- [ ] 所有图片有描述性 alt 文本
- [ ] 表单控件有关联的 label
- [ ] 颜色不是唯一的信息传达方式
- [ ] 图标按钮有 aria-label
- [ ] 支持 prefers-reduced-motion

---

**文档版本**：v1.0
**最后更新**：2026年2月8日
**适用项目**：大模型应用场景管理系统
**技术栈**：React + Tailwind CSS
