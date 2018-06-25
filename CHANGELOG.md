## Changelog

### previsous version

1. There is a change in InitializeAsync. Please do check it.

2. For parameters, please refer to the document we provide separately.

3. Game Friend APIs are deprecated. Please use PION feature instead.

    List of deprecated APIs
    1. getGameFriends
    2. getSentGameFriendRequests
    3. getReceivedGameFriendRequests
    4. getSuggestGameFriends
    5. sendGameFriendRequest
    6. cancelSentGameFriendRequest
    7. acceptGameFriendRequest
    8. declineGameFriendRequest
    9. removeGameFriend
    10. addFavoriteGameFriend
    11. removeFavoriteGameFriend

4. Now you can use LINE coin and QUICK coin feature with newly added getCoinBalance API and purchaseItem API. You need itemId to use the APIs. Please contact LINE Game Tech team for itemId. Please refer to Player section for further details.

5. Fixed a bug where error callback did not come when initializeAsync call failed.

7. Fixed a bug where QUICK navigation is centered.

8. getPhotoUrl no longer returns Object type profile information even for the users without profile picture.

9. The event codes ON_CHANGE_BACKGROUND and ON_CHNAGE_FOREGROUND are currently being tested for usability. We need your opinion for improvements. Please share us your opinion.

### 0.6.7

1. getPlatform API has been deprecated.

2. The parameter value of postTimeline has been simplified. Please refer to the document for details.

3. getAccessToken has been added to Player class. You no longer need to access private member variables.

4. UI class has been created. The showLoadingbar, hideLoadingbar, and setProgress methods that were previously called from an instance should be called on the UI class. For more information, please refer to the UI section below.

5. Fixed an issue where the code value was not provided separately from the error. You can now define the contents of the error code with error.code.

6. getGameFriends API has been added to the Player class. Permission is required to use this API. Please contact tech PM for the permission.

7. Some version compatibility issues have been fixed.

### 0.7.2

1. QUICK coin related feature is no longer provided.
2. We now provide gzip compression version.
3. SDK is now using core-js instead of babel-polyfill.

### 0.8.10

1. getBalance can acquire the QUICK Coin value again.
2. PurchaseItem is deleted from client SDk due to security issue. A Server API guide has been added.
3. showQUICKCoinHistory, showLINECoinHistory APIs have been added.
4. showBillingMethodPage, hideBillingMethodPage, showBillingSuccessPage, hideBillingSuccessPage APIs have been added.
5. user permission, policy check have been added to the initializeAsync entry. They are automatically called upon initializeAsync call.
6. getFriends API는 현재 사용이 불가능합니다. 이후 버전에서 API제공 예정입니다.
