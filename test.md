      .circle {
        width: 20px;
        height: 20px;
        background: radial-gradient(var(--color-main), var(--color-primary), var(--color-secondary));
        border-radius: 50%;
        position: absolute;
        top: 0;
        left: 0;
        animation: rotateAroundBorder 10s linear infinite;
      }
      @keyframes rotateAroundBorder {
        0%, 100% {
            top: 0;
            left: 0;
        }
        25% {
            top: 0;
            left: 100%;
            transform: translateX(-100%);
        }
        50% {
            top: 100%;
            left: 100%;
            transform: translate(-100%, -100%);
        }
        75% {
            top: 100%;
            left: 0;
            transform: translateY(-100%);
        }
      }
