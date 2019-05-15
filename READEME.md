# 一个机遇vue简单倒计时

特点


    - 使用简单,只有两个属性
    - 倒计时持久化，及时页面刷新，倒计时依然我行我素。
   
   
下载   

    ```
    npm i e-countdown
    yarn add "vue-countdown"
    ``` 
     
使用
    
    ``index.vue``
    
    ```
    //t-key防止倒计时和之前的关联
    template
        vue-countdown(v-model="countdown" :t-key="xxxx")
    script
        {
            data(){
                return {
                    countdown:0,
                }
            },
            
            methods: {
                /*
                 * 开始倒计时 当倒计时value=0==0的时候停止倒计时
                 */
                startCountdown(){
                    this.countdown = 10;
                },
                
                
                /*
                 * 停止
                 */
                stopCountdown(){
                    this.countdown = 0;

                },
            }
            
        }
    ```