#include <iostream>
#include <cstdlib> // 用于 rand() 和 srand()
#include <ctime>   // 用于 time()
using namespace std;

int main() {
    // 初始化随机数种子
    srand(time(0));
    
    // 生成1到100的随机数
    int secretNumber = rand() % 100 + 1;
    int guess;
    int attempts = 0;
    
    cout << "欢迎体验猜数字游戏！" << endl;
    cout << "请输入1到100之间的数字，尝试猜出神秘数字！" << endl;
    
    do {
        cout << "请输入你的猜测: ";
        cin >> guess;
        attempts++;
        
        if (guess > secretNumber) {
            cout << "太大了！再试一次。" << endl;
        } else if (guess < secretNumber) {
            cout << "太小了！再试一次。" << endl;
        } else {
            cout << "恭喜你！猜对了！神秘数字是 " << secretNumber << endl;
            cout << "你用了 " << attempts << " 次尝试。" << endl;
        }
    } while (guess != secretNumber);
    
    return 0;
}
