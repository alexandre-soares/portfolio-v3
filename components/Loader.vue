<template>
  <Transition>
    <div class="loader__wrapper">
      <div class="loader">
        <svg
          id="mainSVG"
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 800 600"
        >
          <defs>
            <filter id="drop" x="-100%" y="-100%" width="250%" height="250%">
              <feGaussianBlur stdDeviation="5" result="coloredBlur" />
              <feOffset dx="0" dy="60" result="offsetblur"></feOffset>
              <feFlood
                id="glowAlpha"
                flood-color="#555"
                flood-opacity="0.12"
              ></feFlood>
              <feComposite in2="offsetblur" operator="in"></feComposite>
              <feMerge>
                <feMergeNode />
                <feMergeNode in="SourceGraphic"></feMergeNode>
              </feMerge>
            </filter>

            <filter id="drop2" x="-100%" y="-100%" width="250%" height="250%">
              <feGaussianBlur stdDeviation="6" result="coloredBlur" />
              <feOffset dx="0" dy="6" result="offsetblur"></feOffset>
              <feFlood
                id="glowAlpha"
                flood-color="#555"
                flood-opacity="0.51"
              ></feFlood>
              <feComposite in2="offsetblur" operator="in"></feComposite>
              <feMerge>
                <feMergeNode />
                <feMergeNode in="SourceGraphic"></feMergeNode>
              </feMerge>
            </filter>

            <filter id="goo">
              <feGaussianBlur
                in="SourceGraphic"
                stdDeviation="7"
                result="blur"
              />
              <feColorMatrix
                in="blur"
                mode="matrix"
                values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 21 -9"
                result="cm"
              />
              <feBlend />
            </filter>
            <linearGradient
              id="grad1"
              gradientUnits="userSpaceOnUse"
              x1="400"
              y1="100"
              x2="400"
              y2="600"
            >
              <stop offset="0" style="stop-color: #059ff6" />
              <stop offset="1" style="stop-color: #0369f3" />
            </linearGradient>
            <path id="copyright-cg" d="" />
            <linearGradient
              id="grad2"
              gradientUnits="userSpaceOnUse"
              x1="400"
              y1="200"
              x2="400"
              y2="400"
            >
              <stop offset="0" style="stop-color: #059ff6" />
              <stop offset="1" style="stop-color: #0408a7" />
            </linearGradient>
            <linearGradient
              id="grad3"
              gradientUnits="userSpaceOnUse"
              x1="400"
              y1="500"
              x2="400"
              y2="600"
            >
              <stop offset="0" style="stop-color: #059ff6" />
              <stop offset="1" style="stop-color: #0369f3" />
            </linearGradient>

            <linearGradient
              id="grad4"
              gradientUnits="userSpaceOnUse"
              x1="400"
              y1="200"
              x2="400"
              y2="300"
            >
              <stop offset="0" style="stop-color: #02dbfe" />
              <stop offset="1" style="stop-color: #0369f3" />
            </linearGradient>

            <linearGradient
              id="grad5"
              gradientUnits="userSpaceOnUse"
              x1="400"
              y1="100"
              x2="400"
              y2="600"
            >
              <stop offset="0" style="stop-color: #0369f3" />
              <stop offset="1" style="stop-color: #02dbfe" />
            </linearGradient>

            <clipPath id="mainMask">
              <circle cx="400" cy="300" r="100" />
            </clipPath>

            <clipPath id="otherMask">
              <rect x="300" y="0" width="200" height="400" rx="100" ry="100" />
            </clipPath>
          </defs>

          <g filter="url(#drop)">
            <g id="whole" clip-path="url(#mainMask)">
              <g class="dots1" filter="url(#goo)" fill="url(#grad1)">
                <circle
                  class="outline"
                  cx="400"
                  cy="300"
                  r="90"
                  fill="none"
                  stroke="#0369F3"
                  stroke-width="23"
                  stroke-dasharray="160 65"
                />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
              </g>

              <g class="dots2" filter="url(#goo)" fill="url(#grad2)">
                <circle
                  class="outline"
                  cx="400"
                  cy="300"
                  r="90"
                  fill="none"
                  stroke="#0408A7"
                  stroke-width="23"
                  stroke-dasharray="160 40"
                />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
              </g>

              <g class="dots3" filter="url(#goo)" fill="url(#grad3)">
                <circle
                  class="outline"
                  cx="400"
                  cy="300"
                  r="90"
                  fill="none"
                  stroke="url(#grad3)"
                  stroke-width="23"
                  stroke-dasharray="240 "
                />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
              </g>

              <g class="dots4" filter="url(#goo)" fill="url(#grad4)">
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
                <circle class="dot" cx="0" cy="0" r="20" />
              </g>
            </g>
          </g>
          <g filter="url(#drop2)">
            <g clip-path="url(#otherMask)">
              <g class="dots5" fill="url(#grad2)" filter="url(#goo)">
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
                <circle class="outsideDot" cx="0" cy="0" r="20" />
              </g>
            </g>
          </g>
        </svg>
        <p>Loading...</p>
      </div>
    </div>
  </Transition>
</template>

<script>
import gsap from 'gsap'
export default {
  name: 'Loader',
  mounted() {
    gsap.set('svg', {
      visibility: 'visible'
    })
    gsap.set('.dot', {
      transformOrigin: '50% 50%',
      attr: {
        cx: 'random(350, 450)',
        cy: 440,
        r: 'random(4, 20)'
      }
    })
    gsap.set('.outsideDot', {
      transformOrigin: '50% 50%',
      attr: {
        cx: 'random(370, 420)',
        cy: 420,
        r: 'random(3, 19)'
      }
    })
    const tl1 = gsap.timeline()
    tl1
      .to('.dots1 .dot', {
        duration: 'random(2,8)',
        attr: {
          cy: 'random(-220, -320)'
        },
        stagger: {
          each: 0.16,
          repeat: -1,
          repeatRefresh: false
        },
        ease: 'linear'
      })
      .seek(100)

    const tl2 = gsap.timeline()
    tl2
      .to('.dots2 .dot', {
        duration: 'random(2,5)',
        attr: {
          cy: 'random(-220, -320)'
        },
        stagger: {
          each: 0.16,
          repeat: -1,
          repeatRefresh: false
        },
        ease: 'sine.in'
      })
      .seek(100)

    const tl3 = gsap.timeline()
    tl3
      .to('.dots3 .dot', {
        duration: 'random(6,12)',
        attr: {
          cy: 'random(-220, -320)'
        },
        stagger: {
          each: 0.16,
          repeat: -1,
          repeatRefresh: false
        },
        ease: 'sine.in'
      })
      .seek(100)

    const tl4 = gsap.timeline()
    tl4
      .to('.dots4 .dot', {
        duration: 'random(3,9)',
        attr: {
          cy: 'random(-220, -320)'
        },
        stagger: {
          each: 0.16,
          repeat: -1,
          repeatRefresh: false
        },
        ease: 'sine.in'
      })
      .seek(100)

    const tl5 = gsap.timeline()
    tl5
      .to('.dots5 .outsideDot', {
        duration: 'random(3,9)',
        attr: {
          cy: 'random(-220, -320)',
          r: 0
        },
        stagger: {
          each: 0.16,
          repeat: -1,
          repeatRefresh: false
        },
        ease: 'power2.in'
      })
      .seek(100)

    gsap
      .to('.outline', {
        duration: gsap.utils.wrap([7, 6.1, 5.2]),
        svgOrigin: '400 300',
        rotation: gsap.utils.wrap([-360, -360]),
        ease: 'linear',
        stagger: {
          each: 1,
          repeat: -1
        }
      })
      .seek(200)
    // ScrubGSAPTimeline(tl)
    // gsap.globalTimeline.timeScale(0.25);
  }
}
</script>

<style lang="scss" scoped>
.loader {
  &__wrapper {
    position: fixed;
    top: 0;
    left: 0;
    height: 100vh;
    width: 100vw;
    z-index: 9999;
    background-color: #fffcf9;
    overflow: hidden;
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
svg {
  width: 100%;
  height: 100%;
  visibility: hidden;
}

p {
  margin-top: -40px;
  width: 100%;
}

/* we will explain what these classes do next! */
.v-enter-active,
.v-leave-active {
  transition: opacity 0.5s ease;
}

.v-enter-from,
.v-leave-to {
  opacity: 0;
}
</style>
