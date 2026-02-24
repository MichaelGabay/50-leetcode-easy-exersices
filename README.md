# 50 תרגילי LeetCode – רמת Easy

רשימת תרגילים עם קישורים ל-LeetCode ופתרונות Python בסוף המסמך.

---

## רשימת התרגילים

### 1. Two Sum
**קישור:** https://leetcode.com/problems/two-sum/  
**תיאור:** מצא שני מספרים במערך שסכומם שווה ל-target. החזר אינדקסים.  
**דוגמאות:**  
- תקין: `nums = [2, 7, 11, 15], target = 9` → `[0, 1]` (כי 2+7=9).  
- תקין: `nums = [3, 2, 4], target = 6` → `[1, 2]`.  
- לא תקין: אין פתרון – מובטח שיש בדיוק פתרון אחד.

### 2. Palindrome Number
**קישור:** https://leetcode.com/problems/palindrome-number/  
**תיאור:** קבע אם מספר שלם הוא פלינדרום (נקרא אותו משני הצדדים).  
**דוגמאות:**  
- תקין: `121` → `True`. `12321` → `True`.  
- לא תקין: `-121` → `False` (מינוס). `10` → `False`.

### 3. Roman to Integer
**קישור:** https://leetcode.com/problems/roman-to-integer/  
**תיאור:** המר מחרוזת ספרות רומיות למספר שלם.  
**דוגמאות:**  
- תקין: `"III"` → `3`. `"LVIII"` → `58`. `"MCMXCIV"` → `1994`.  
- לא רלוונטי: הקלט תמיד תקין (I,V,X,L,C,D,M).

### 4. Longest Common Prefix
**קישור:** https://leetcode.com/problems/longest-common-prefix/  
**תיאור:** מצא את התחילית המשותפת הארוכה ביותר בין מחרוזות במערך.  
**דוגמאות:**  
- תקין: `["flower","flow","flight"]` → `"fl"`. `["dog","racecar","car"]` → `""`.  
- קצה: `["a"]` → `"a"`. `[]` → `""`.

### 5. Valid Parentheses
**קישור:** https://leetcode.com/problems/valid-parentheses/  
**תיאור:** בדוק אם מחרוזת סוגריים ( ) [ ] { } תקינה – כל סוגר נסגר בסדר נכון.  
**דוגמאות:**  
- תקין: `"()"` → `True`. `"()[]{}"` → `True`. `"{[]}"` → `True`.  
- לא תקין: `"(]"` → `False`. `"([)]"` → `False`. `"("` → `False`.

### 6. Merge Two Sorted Lists
**קישור:** https://leetcode.com/problems/merge-two-sorted-lists/  
**תיאור:** מיזוג שני רשימות מקושרות ממוינות לרשימה אחת ממוינת.  
**דוגמאות:**  
- תקין: `[1,2,4]` + `[1,3,4]` → `[1,1,2,3,4,4]`.  
- קצה: `[]` + `[0]` → `[0]`. שתי רשימות ריקות → `[]`.

### 7. Remove Duplicates from Sorted Array
**קישור:** https://leetcode.com/problems/remove-duplicates-from-sorted-array/  
**תיאור:** הסר כפילויות ממערך ממוין in-place, החזר אורך החלק הייחודי.  
**דוגמאות:**  
- תקין: `[1,1,2]` → אורך `2`, המערך מתחיל ב-`[1,2,...]`.  
- תקין: `[0,0,1,1,1,2,2,3,3,4]` → אורך `5`, `[0,1,2,3,4,...]`.  
- לא תקין: אין – הקלט תמיד מערך ממוין.

### 8. Implement strStr()
**קישור:** https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/  
**תיאור:** מצא את האינדקס של ההופעה הראשונה של needle ב-haystack (או -1).  
**דוגמאות:**  
- תקין: `haystack = "sadbutsad", needle = "sad"` → `0`. `"leetcode", "leeto"` → `-1`.  
- קצה: `needle = ""` → `0`. `"aaa", "aaaa"` → `-1`.

### 9. Search Insert Position
**קישור:** https://leetcode.com/problems/search-insert-position/  
**תיאור:** מצא את האינדקס שבו יש להכניס target במערך ממוין (או איפה שהוא כבר קיים).  
**דוגמאות:**  
- תקין: `[1,3,5,6], target = 5` → `2`. `[1,3,5,6], target = 2` → `1`.  
- תקין: `[1,3,5,6], target = 7` → `4`. `[1,3,5,6], target = 0` → `0`.

### 10. Maximum Subarray (Kadane)
**קישור:** https://leetcode.com/problems/maximum-subarray/  
**תיאור:** מצא את תת-המערך הרציף עם הסכום המקסימלי.  
**דוגמאות:**  
- תקין: `[-2,1,-3,4,-1,2,1,-5,4]` → `6` (תת-מערך `[4,-1,2,1]`).  
- תקין: `[1]` → `1`. `[5,4,-1,7,8]` → `23` (כל המערך).

### 11. Length of Last Word
**קישור:** https://leetcode.com/problems/length-of-last-word/  
**תיאור:** החזר את אורך המילה האחרונה במחרוזת (מילים מופרדות ברווחים).  
**דוגמאות:**  
- תקין: `"Hello World"` → `5`. `"   fly me   to   the moon  "` → `4`.  
- קצה: `"a"` → `1`. מחרוזת רווחים בלבד → `0`.

### 12. Plus One
**קישור:** https://leetcode.com/problems/plus-one/  
**תיאור:** ייצג מספר כמערך ספרות, הוסף 1 והחזר את המערך המעודכן.  
**דוגמאות:**  
- תקין: `[1,2,3]` → `[1,2,4]`. `[4,3,2,1]` → `[4,3,2,2]`.  
- קצה: `[9]` → `[1,0]`. `[9,9,9]` → `[1,0,0,0]`.

### 13. Climbing Stairs
**קישור:** https://leetcode.com/problems/climbing-stairs/  
**תיאור:** בכמה דרכים אפשר לטפס n מדרגות (1 או 2 בכל צעד)?  
**דוגמאות:**  
- תקין: `n = 2` → `2` (1+1 או 2). `n = 3` → `3`. `n = 4` → `5`.  
- קצה: `n = 1` → `1`.

### 14. Merge Sorted Array
**קישור:** https://leetcode.com/problems/merge-sorted-array/  
**תיאור:** מיזוג nums2 ל-nums1 (ל-nums1 יש מקום בסוף). מיזוג in-place.  
**דוגמאות:**  
- תקין: `nums1 = [1,2,3,0,0,0], m = 3`, `nums2 = [2,5,6], n = 3` → nums1 הופך ל-`[1,2,2,3,5,6]`.  
- קצה: `nums1 = [1], m = 1`, `nums2 = [], n = 0` → נשאר `[1]`.

### 15. Symmetric Tree
**קישור:** https://leetcode.com/problems/symmetric-tree/  
**תיאור:** בדוק אם העץ בינארי סימטרי סביב המרכז (מראה).  
**דוגמאות:**  
- תקין: עץ עם שורש וילדים 2,2 ו-3,3 בשכבה הבאה → `True`.  
- לא תקין: `[1,2,2,null,3,null,3]` → `False`. עץ ריק → `True`.

### 16. Maximum Depth of Binary Tree
**קישור:** https://leetcode.com/problems/maximum-depth-of-binary-tree/  
**תיאור:** מצא את עומק העץ הבינארי (מספר הרמות, שורש = 1).  
**דוגמאות:**  
- תקין: `[3,9,20,null,null,15,7]` → `3`. `[1,null,2]` → `2`.  
- קצה: `[]` → `0`. צומת בודד → `1`.

### 17. Same Tree
**קישור:** https://leetcode.com/problems/same-tree/  
**תיאור:** בדוק אם שני עצים בינאריים זהים (מבנה וערכים).  
**דוגמאות:**  
- תקין: `[1,2,3]` ו-`[1,2,3]` → `True`.  
- לא תקין: `[1,2]` ו-`[1,null,2]` → `False`. `[1,2,1]` ו-`[1,1,2]` → `False`.

### 18. Invert Binary Tree
**קישור:** https://leetcode.com/problems/invert-binary-tree/  
**תיאור:** הפוך את העץ – החלף שמאל וימין בכל צומת.  
**דוגמאות:**  
- תקין: `[4,2,7,1,3,6,9]` → `[4,7,2,9,6,3,1]`.  
- קצה: `[]` → `[]`. צומת בודד → ללא שינוי.

### 19. Single Number
**קישור:** https://leetcode.com/problems/single-number/  
**תיאור:** במערך כל מספר מופיע פעמיים חוץ מאחד. מצא את המספר היחיד (O(n) זמן, O(1) מקום).  
**דוגמאות:**  
- תקין: `[2,2,1]` → `1`. `[4,1,2,1,2]` → `4`.  
- קצה: `[1]` → `1`.

### 20. Move Zeroes
**קישור:** https://leetcode.com/problems/move-zeroes/  
**תיאור:** הזז את כל האפסים לסוף המערך in-place (שנה את המערך, אין החזרה).  
**דוגמאות:**  
- תקין: `[0,1,0,3,12]` → המערך הופך ל-`[1,3,12,0,0]`.  
- תקין: `[0,0,1]` → `[1,0,0]`. אין אפסים → ללא שינוי.

### 21. Best Time to Buy and Sell Stock
**קישור:** https://leetcode.com/problems/best-time-to-buy-and-sell-stock/  
**תיאור:** מצא את הרווח המקסימלי (קנייה ביום אחד, מכירה ביום מאוחר יותר – עסקה אחת).  
**דוגמאות:**  
- תקין: `[7,1,5,3,6,4]` → `5` (קנייה ב-1, מכירה ב-6).  
- לא רווח: `[7,6,4,3,1]` → `0`. מערך ריק → `0`.

### 22. Majority Element
**קישור:** https://leetcode.com/problems/majority-element/  
**תיאור:** מצא אלמנט שמופיע יותר מ-n/2 פעמים (מובטח שקיים).  
**דוגמאות:**  
- תקין: `[3,2,3]` → `3`. `[2,2,1,1,1,2,2]` → `2`.  
- קצה: `[1]` → `1`.

### 23. Reverse Linked List
**קישור:** https://leetcode.com/problems/reverse-linked-list/  
**תיאור:** הפוך רשימה מקושרת (iterative או recursive). החזר ראש הרשימה החדשה.  
**דוגמאות:**  
- תקין: `1→2→3→null` → `3→2→1→null`.  
- קצה: `[]` → `[]`. צומת בודד → אותו צומת.

### 24. Contains Duplicate
**קישור:** https://leetcode.com/problems/contains-duplicate/  
**תיאור:** בדוק אם יש במערך אלמנט שמופיע לפחות פעמיים.  
**דוגמאות:**  
- תקין: `[1,2,3,1]` → `True`. `[1,2,3,4]` → `False`.  
- קצה: `[1,1,1,1]` → `True`.

### 25. Missing Number
**קישור:** https://leetcode.com/problems/missing-number/  
**תיאור:** מערך מכיל בדיוק את המספרים מ-0 עד n, חסר מספר אחד. מצא אותו.  
**דוגמאות:**  
- תקין: `[3,0,1]` → `2`. `[0,1]` → `2`. `[9,6,4,2,3,5,7,0,1]` → `8`.  
- קצה: `[0]` → `1`.

### 26. Intersection of Two Arrays II
**קישור:** https://leetcode.com/problems/intersection-of-two-arrays-ii/  
**תיאור:** החזר חיתוך של שני מערכים – כל אלמנט שמופיע בשניהם, עם כפילויות לפי המינימום.  
**דוגמאות:**  
- תקין: `[1,2,2,1]`, `[2,2]` → `[2,2]`. `[4,9,5]`, `[9,4,9,8,4]` → `[4,9]` או `[9,4]`.  
- קצה: אין חיתוך → `[]`.

### 27. First Unique Character in a String
**קישור:** https://leetcode.com/problems/first-unique-character-in-a-string/  
**תיאור:** מצא את האינדקס של התו הראשון שמופיע רק פעם אחת.  
**דוגמאות:**  
- תקין: `"leetcode"` → `0` (l). `"loveleetcode"` → `2` (v).  
- לא קיים: `"aabb"` → `-1`.

### 28. Valid Anagram
**קישור:** https://leetcode.com/problems/valid-anagram/  
**תיאור:** בדוק אם s ו-t אנגרמות (אותן אותיות באותו כמות, סדר שונה).  
**דוגמאות:**  
- תקין: `"anagram"`, `"nagaram"` → `True`.  
- לא תקין: `"rat"`, `"car"` → `False`. אורכים שונים → `False`.

### 29. Reverse String
**קישור:** https://leetcode.com/problems/reverse-string/  
**תיאור:** הפוך את המחרוזת in-place (מערך תווים – שינוי במקום, אין החזרה).  
**דוגמאות:**  
- תקין: `["h","e","l","l","o"]` → המערך `["o","l","l","e","h"]`.  
- קצה: `["a","b"]` → `["b","a"]`.

### 30. Binary Search
**קישור:** https://leetcode.com/problems/binary-search/  
**תיאור:** מצא את target במערך ממוין. החזר אינדקס או -1. O(log n).  
**דוגמאות:**  
- תקין: `[-1,0,3,5,9,12], target = 9` → `4`. `[-1,0,3,5,9,12], target = 2` → `-1`.  
- קצה: `[5], target = 5` → `0`.

### 31. First Bad Version
**קישור:** https://leetcode.com/problems/first-bad-version/  
**תיאור:** גרסאות 1..n, מ-position מסוים כולן רעות. מצא את הגרסה הראשונה הרעה (binary search).  
**דוגמאות:**  
- תקין: `n = 5`, גרסה 4 היא הראשונה הרעה → `4`.  
- קצה: רק גרסה 1 רעה → `1`. רק גרסה n רעה → `n`.

### 32. Sqrt(x)
**קישור:** https://leetcode.com/problems/sqrtx/  
**תיאור:** החזר שורש ריבועי מעוגל למטה (ללא פונקציות מובנות).  
**דוגמאות:**  
- תקין: `4` → `2`. `8` → `2` (2.828... מעוגל ל-2).  
- קצה: `0` → `0`. `1` → `1`.

### 33. Pascal's Triangle
**קישור:** https://leetcode.com/problems/pascals-triangle/  
**תיאור:** בנה משולש פסקל עם numRows שורות (כל שורה מתחילה ונגמרת ב-1).  
**דוגמאות:**  
- תקין: `numRows = 5` → `[[1],[1,1],[1,2,1],[1,3,3,1],[1,4,6,4,1]]`.  
- קצה: `numRows = 1` → `[[1]]`. `0` → `[]`.

### 34. Best Time to Buy and Sell Stock II
**קישור:** https://leetcode.com/problems/best-time-to-buy-and-sell-stock-ii/  
**תיאור:** רווח מקסימלי עם מספר עסקאות (אפשר לקנות ולמכור כמה פעמים).  
**דוגמאות:**  
- תקין: `[7,1,5,3,6,4]` → `7` (קנה 1 מכר 5, קנה 3 מכר 6).  
- תקין: `[1,2,3,4,5]` → `4`. `[7,6,4,3,1]` → `0`.

### 35. Valid Palindrome
**קישור:** https://leetcode.com/problems/valid-palindrome/  
**תיאור:** בדוק אם מחרוזת היא פלינדרום – רק אותיות וספרות, התעלם מרווחים וסימנים.  
**דוגמאות:**  
- תקין: `"A man, a plan, a canal: Panama"` → `True`. `"race a car"` → `False`.  
- קצה: `" "` → `True`. `"0P"` → `False` (0 ו-P).

### 36. Linked List Cycle
**קישור:** https://leetcode.com/problems/linked-list-cycle/  
**תיאור:** בדוק אם יש cycle ברשימה המקושרת (next מצביע אחורה לצומת קודם).  
**דוגמאות:**  
- תקין: רשימה עם cycle (למשל tail.next = head) → `True`.  
- לא תקין: רשימה שמסתיימת ב-null → `False`. רשימה ריקה → `False`.

### 37. Min Stack
**קישור:** https://leetcode.com/problems/min-stack/  
**תיאור:** מחסנית שתומכת ב-push, pop, top ו-getMin – כולן ב-O(1).  
**דוגמאות:**  
- תקין: push(-2), push(0), push(-3), getMin() → -3; pop(); top() → 0; getMin() → -2.  
- לא רלוונטי: התנהגות מוגדרת לכל פעולה.

### 38. Intersection of Two Linked Lists
**קישור:** https://leetcode.com/problems/intersection-of-two-linked-lists/  
**תיאור:** מצא את הצומת הראשון המשותף (by reference) של שתי הרשימות, או null.  
**דוגמאות:**  
- תקין: listA = 4→1→8→4→5, listB = 5→6→1→8→4→5 (משותף מ-8) → החזר צומת 8.  
- לא מפגש: שתי רשימות נפרדות → `null`.

### 39. Excel Sheet Column Title
**קישור:** https://leetcode.com/problems/excel-sheet-column-title/  
**תיאור:** המר מספר עמודה (1=A, 2=B, ..., 26=Z, 27=AA) למחרוזת.  
**דוגמאות:**  
- תקין: `1` → `"A"`. `28` → `"AB"`. `701` → `"ZY"`.  
- לא תקין: `0` לא נתון (רק חיוביים).

### 40. Majority Element II
**קישור:** https://leetcode.com/problems/majority-element-ii/  
**תיאור:** מצא את כל האלמנטים שמופיעים יותר מ-n/3 פעמים (יכולים 0, 1 או 2).  
**דוגמאות:**  
- תקין: `[3,2,3]` → `[3]`. `[1]` → `[1]`. `[1,2]` → `[1,2]`.  
- אין: `[1,2,3,4]` → `[]`.

### 41. Power of Two
**קישור:** https://leetcode.com/problems/power-of-two/  
**תיאור:** בדוק אם n הוא חזקה של 2 (1, 2, 4, 8, ...).  
**דוגמאות:**  
- תקין: `1` → `True`. `16` → `True`.  
- לא תקין: `3` → `False`. `0` → `False`. `-2` → `False`.

### 42. Add Digits
**קישור:** https://leetcode.com/problems/add-digits/  
**תיאור:** "Digital root" – סכום ספרות, חוזר עד שמגיעים לספרה אחת (0..9).  
**דוגמאות:**  
- תקין: `38` → 3+8=11 → 1+1=2 → `2`. `0` → `0`.  
- תקין: `123` → 1+2+3=6 → `6`.

### 43. Ugly Number
**קישור:** https://leetcode.com/problems/ugly-number/  
**תיאור:** בדוק אם המספר (חיובי) מחולק רק ב-2, 3, 5 (כולל 1).  
**דוגמאות:**  
- תקין: `6` → `True`. `1` → `True`. `14` → `False` (7).  
- לא תקין: `0` → `False`. `-6` → `False`.

### 44. Word Pattern
**קישור:** https://leetcode.com/problems/word-pattern/  
**תיאור:** התאמה 1:1: כל אות ב-pattern ממופה למילה אחת ב-str ולהפך.  
**דוגמאות:**  
- תקין: `pattern = "abba"`, `str = "dog cat cat dog"` → `True`.  
- לא תקין: `"abba"`, `"dog cat cat fish"` → `False`. `"aaaa"`, `"dog cat cat dog"` → `False`.

### 45. Nim Game
**קישור:** https://leetcode.com/problems/nim-game/  
**תיאור:** n אבנים, כל תור לוקחים 1–3. אתה מתחיל. החזר True אם יש לך אסטרטגיה מנצחת.  
**דוגמאות:**  
- תקין: `n = 4` → `False` (השחקן השני ינצח). `n = 1,2,3` → `True`.  
- תקין: `n = 5` → `True` (תיקח 1, יישארו 4).

### 46. Range Sum Query - Immutable
**קישור:** https://leetcode.com/problems/range-sum-query-immutable/  
**תיאור:** נתון מערך – בנה מבנה שמאפשר שאילתות סכום [left, right] ב-O(1).  
**דוגמאות:**  
- תקין: מערך `[-2, 0, 3, -5, 2, -1]`, sumRange(0,2) → 1, sumRange(2,5) → -1, sumRange(0,5) → -3.  
- קצה: sumRange(i,i) → nums[i].

### 47. Pascal's Triangle II
**קישור:** https://leetcode.com/problems/pascals-triangle-ii/  
**תיאור:** החזר רק את שורת המשולש של פסקל באינדקס rowIndex (0-based), ב-O(rowIndex) מקום.  
**דוגמאות:**  
- תקין: `rowIndex = 3` → `[1,3,3,1]`. `rowIndex = 0` → `[1]`.  
- תקין: `rowIndex = 1` → `[1,1]`.

### 48. Contains Duplicate II
**קישור:** https://leetcode.com/problems/contains-duplicate-ii/  
**תיאור:** בדוק אם יש זוג אינדקסים i, j כך ש-nums[i]==nums[j] ו-|i-j| ≤ k.  
**דוגמאות:**  
- תקין: `[1,2,3,1], k = 3` → `True` (אינדקסים 0 ו-3). `[1,0,1,1], k = 1` → `True`.  
- לא תקין: `[1,2,3,1], k = 2` → `False`. `[1,2,3,4], k = 1` → `False`.

### 49. Summary Ranges
**קישור:** https://leetcode.com/problems/summary-ranges/  
**תיאור:** מערך ממוין של מספרים ייחודיים – החזר רשימת טווחים: "a->b" או "a" לטווח בן מספר אחד.  
**דוגמאות:**  
- תקין: `[0,1,2,4,5,7]` → `["0->2","4->5","7"]`. `[0,2,3,4,6,8,9]` → `["0","2->4","6","8->9"]`.  
- קצה: `[]` → `[]`. `[1]` → `["1"]`.

### 50. Happy Number
**קישור:** https://leetcode.com/problems/happy-number/  
**תיאור:** מספר "שמח" אם חישוב חוזר של סכום ריבועי הספרות מגיע ל-1; אחרת נכנסים לולאה.  
**דוגמאות:**  
- תקין: `19` → 1²+9²=82 → 68 → 100 → 1 → `True`. `2` → 4 → 16 → 37 → ... (לולאה) → `False`.  
- קצה: `1` → `True`.

---

# פתרונות (Python)

## 1. Two Sum
```python
def twoSum(nums, target):
    seen = {}
    for i, n in enumerate(nums):
        need = target - n
        if need in seen:
            return [seen[need], i]
        seen[n] = i
    return []
```

## 2. Palindrome Number
```python
def isPalindrome(x):
    if x < 0:
        return False
    s = str(x)
    return s == s[::-1]
```

## 3. Roman to Integer
```python
def romanToInt(s):
    d = {'I': 1, 'V': 5, 'X': 10, 'L': 50, 'C': 100, 'D': 500, 'M': 1000}
    total = 0
    for i in range(len(s)):
        if i + 1 < len(s) and d[s[i]] < d[s[i + 1]]:
            total -= d[s[i]]
        else:
            total += d[s[i]]
    return total
```

## 4. Longest Common Prefix
```python
def longestCommonPrefix(strs):
    if not strs:
        return ""
    prefix = strs[0]
    for s in strs[1:]:
        while not s.startswith(prefix):
            prefix = prefix[:-1]
            if not prefix:
                return ""
    return prefix
```

## 5. Valid Parentheses
```python
def isValid(s):
    stack = []
    pair = {')': '(', ']': '[', '}': '{'}
    for c in s:
        if c in pair:
            if not stack or stack[-1] != pair[c]:
                return False
            stack.pop()
        else:
            stack.append(c)
    return len(stack) == 0
```

## 6. Merge Two Sorted Lists
```python
def mergeTwoLists(l1, l2):
    dummy = ListNode(0)
    cur = dummy
    while l1 and l2:
        if l1.val <= l2.val:
            cur.next = l1
            l1 = l1.next
        else:
            cur.next = l2
            l2 = l2.next
        cur = cur.next
    cur.next = l1 or l2
    return dummy.next
```

## 7. Remove Duplicates from Sorted Array
```python
def removeDuplicates(nums):
    if not nums:
        return 0
    k = 1
    for i in range(1, len(nums)):
        if nums[i] != nums[k - 1]:
            nums[k] = nums[i]
            k += 1
    return k
```

## 8. Implement strStr()
```python
def strStr(haystack, needle):
    if not needle:
        return 0
    n, m = len(haystack), len(needle)
    for i in range(n - m + 1):
        if haystack[i:i + m] == needle:
            return i
    return -1
```

## 9. Search Insert Position
```python
def searchInsert(nums, target):
    lo, hi = 0, len(nums) - 1
    while lo <= hi:
        mid = (lo + hi) // 2
        if nums[mid] == target:
            return mid
        if nums[mid] < target:
            lo = mid + 1
        else:
            hi = mid - 1
    return lo
```

## 10. Maximum Subarray
```python
def maxSubArray(nums):
    best = cur = nums[0]
    for x in nums[1:]:
        cur = max(x, cur + x)
        best = max(best, cur)
    return best
```

## 11. Length of Last Word
```python
def lengthOfLastWord(s):
    return len(s.strip().split()[-1]) if s.strip() else 0
```

## 12. Plus One
```python
def plusOne(digits):
    for i in range(len(digits) - 1, -1, -1):
        if digits[i] < 9:
            digits[i] += 1
            return digits
        digits[i] = 0
    return [1] + digits
```

## 13. Climbing Stairs
```python
def climbStairs(n):
    a, b = 1, 1
    for _ in range(n - 1):
        a, b = b, a + b
    return b
```

## 14. Merge Sorted Array
```python
def merge(nums1, m, nums2, n):
    i, j, k = m - 1, n - 1, m + n - 1
    while j >= 0:
        if i >= 0 and nums1[i] > nums2[j]:
            nums1[k] = nums1[i]
            i -= 1
        else:
            nums1[k] = nums2[j]
            j -= 1
        k -= 1
```

## 15. Symmetric Tree
```python
def isSymmetric(root):
    def mirror(l, r):
        if not l and not r:
            return True
        if not l or not r or l.val != r.val:
            return False
        return mirror(l.left, r.right) and mirror(l.right, r.left)
    return mirror(root, root) if root else True
```

## 16. Maximum Depth of Binary Tree
```python
def maxDepth(root):
    if not root:
        return 0
    return 1 + max(maxDepth(root.left), maxDepth(root.right))
```

## 17. Same Tree
```python
def isSameTree(p, q):
    if not p and not q:
        return True
    if not p or not q or p.val != q.val:
        return False
    return isSameTree(p.left, q.left) and isSameTree(p.right, q.right)
```

## 18. Invert Binary Tree
```python
def invertTree(root):
    if not root:
        return None
    root.left, root.right = invertTree(root.right), invertTree(root.left)
    return root
```

## 19. Single Number
```python
def singleNumber(nums):
    res = 0
    for n in nums:
        res ^= n
    return res
```

## 20. Move Zeroes
```python
def moveZeroes(nums):
    j = 0
    for i in range(len(nums)):
        if nums[i] != 0:
            nums[j], nums[i] = nums[i], nums[j]
            j += 1
```

## 21. Best Time to Buy and Sell Stock
```python
def maxProfit(prices):
    if not prices:
        return 0
    best = 0
    low = prices[0]
    for p in prices[1:]:
        best = max(best, p - low)
        low = min(low, p)
    return best
```

## 22. Majority Element
```python
def majorityElement(nums):
    count = 0
    cand = None
    for n in nums:
        if count == 0:
            cand = n
        count += 1 if n == cand else -1
    return cand
```

## 23. Reverse Linked List
```python
def reverseList(head):
    prev = None
    while head:
        nxt = head.next
        head.next = prev
        prev = head
        head = nxt
    return prev
```

## 24. Contains Duplicate
```python
def containsDuplicate(nums):
    return len(nums) != len(set(nums))
```

## 25. Missing Number
```python
def missingNumber(nums):
    n = len(nums)
    return n * (n + 1) // 2 - sum(nums)
```

## 26. Intersection of Two Arrays II
```python
def intersect(nums1, nums2):
    from collections import Counter
    c = Counter(nums1)
    out = []
    for x in nums2:
        if c[x] > 0:
            out.append(x)
            c[x] -= 1
    return out
```

## 27. First Unique Character in a String
```python
def firstUniqChar(s):
    from collections import Counter
    c = Counter(s)
    for i, ch in enumerate(s):
        if c[ch] == 1:
            return i
    return -1
```

## 28. Valid Anagram
```python
def isAnagram(s, t):
    return sorted(s) == sorted(t)
# או: return Counter(s) == Counter(t)
```

## 29. Reverse String
```python
def reverseString(s):
    i, j = 0, len(s) - 1
    while i < j:
        s[i], s[j] = s[j], s[i]
        i += 1
        j -= 1
```

## 30. Binary Search
```python
def search(nums, target):
    lo, hi = 0, len(nums) - 1
    while lo <= hi:
        mid = (lo + hi) // 2
        if nums[mid] == target:
            return mid
        if nums[mid] < target:
            lo = mid + 1
        else:
            hi = mid - 1
    return -1
```

## 31. First Bad Version
```python
def firstBadVersion(n):
    lo, hi = 1, n
    while lo < hi:
        mid = (lo + hi) // 2
        if isBadVersion(mid):
            hi = mid
        else:
            lo = mid + 1
    return lo
```

## 32. Sqrt(x)
```python
def mySqrt(x):
    if x < 2:
        return x
    lo, hi = 0, x
    while lo <= hi:
        mid = (lo + hi) // 2
        if mid * mid <= x < (mid + 1) ** 2:
            return mid
        if mid * mid > x:
            hi = mid - 1
        else:
            lo = mid + 1
    return lo
```

## 33. Pascal's Triangle
```python
def generate(numRows):
    if numRows == 0:
        return []
    res = [[1]]
    for i in range(1, numRows):
        row = [1]
        for j in range(1, i):
            row.append(res[-1][j - 1] + res[-1][j])
        row.append(1)
        res.append(row)
    return res
```

## 34. Best Time to Buy and Sell Stock II
```python
def maxProfit(prices):
    profit = 0
    for i in range(1, len(prices)):
        if prices[i] > prices[i - 1]:
            profit += prices[i] - prices[i - 1]
    return profit
```

## 35. Valid Palindrome
```python
def isPalindrome(s):
    s = ''.join(c.lower() for c in s if c.isalnum())
    return s == s[::-1]
```

## 36. Linked List Cycle
```python
def hasCycle(head):
    slow = fast = head
    while fast and fast.next:
        slow = slow.next
        fast = fast.next.next
        if slow == fast:
            return True
    return False
```

## 37. Min Stack
```python
class MinStack:
    def __init__(self):
        self.stack = []
        self.min_stack = []

    def push(self, val):
        self.stack.append(val)
        if not self.min_stack or val <= self.min_stack[-1]:
            self.min_stack.append(val)

    def pop(self):
        if self.stack.pop() == self.min_stack[-1]:
            self.min_stack.pop()

    def top(self):
        return self.stack[-1]

    def getMin(self):
        return self.min_stack[-1]
```

## 38. Intersection of Two Linked Lists
```python
def getIntersectionNode(headA, headB):
    a, b = headA, headB
    while a != b:
        a = a.next if a else headB
        b = b.next if b else headA
    return a
```

## 39. Excel Sheet Column Title
```python
def convertToTitle(columnNumber):
    s = ""
    while columnNumber > 0:
        columnNumber -= 1
        s = chr(ord('A') + columnNumber % 26) + s
        columnNumber //= 26
    return s
```

## 40. Majority Element II
```python
def majorityElement(nums):
    c1 = c2 = 0
    m1 = m2 = None
    for n in nums:
        if n == m1:
            c1 += 1
        elif n == m2:
            c2 += 1
        elif c1 == 0:
            m1, c1 = n, 1
        elif c2 == 0:
            m2, c2 = n, 1
        else:
            c1 -= 1
            c2 -= 1
    return [m for m in (m1, m2) if m is not None and nums.count(m) > len(nums) // 3]
```

## 41. Power of Two
```python
def isPowerOfTwo(n):
    return n > 0 and (n & (n - 1)) == 0
```

## 42. Add Digits
```python
def addDigits(num):
    return 1 + (num - 1) % 9 if num else 0
```

## 43. Ugly Number
```python
def isUgly(n):
    if n <= 0:
        return False
    for p in (2, 3, 5):
        while n % p == 0:
            n //= p
    return n == 1
```

## 44. Word Pattern
```python
def wordPattern(pattern, s):
    words = s.split()
    if len(pattern) != len(words):
        return False
    return len(set(pattern)) == len(set(words)) == len(set(zip(pattern, words)))
```

## 45. Nim Game
```python
def canWinNim(n):
    return n % 4 != 0
```

## 46. Range Sum Query - Immutable
```python
class NumArray:
    def __init__(self, nums):
        self.prefix = [0]
        for x in nums:
            self.prefix.append(self.prefix[-1] + x)

    def sumRange(self, left, right):
        return self.prefix[right + 1] - self.prefix[left]
```

## 47. Pascal's Triangle II
```python
def getRow(rowIndex):
    row = [1]
    for i in range(rowIndex):
        row = [1] + [row[j] + row[j + 1] for j in range(len(row) - 1)] + [1]
    return row
```

## 48. Contains Duplicate II
```python
def containsNearbyDuplicate(nums, k):
    seen = {}
    for i, n in enumerate(nums):
        if n in seen and i - seen[n] <= k:
            return True
        seen[n] = i
    return False
```

## 49. Summary Ranges
```python
def summaryRanges(nums):
    if not nums:
        return []
    res = []
    start = nums[0]
    for i in range(1, len(nums) + 1):
        if i == len(nums) or nums[i] != nums[i - 1] + 1:
            res.append(str(start) if start == nums[i - 1] else f"{start}->{nums[i - 1]}")
            if i < len(nums):
                start = nums[i]
    return res
```

## 50. Happy Number
```python
def isHappy(n):
    seen = set()
    while n != 1 and n not in seen:
        seen.add(n)
        n = sum(int(d) ** 2 for d in str(n))
    return n == 1
```

---

*כל הפתרונות מתאימים להגדרת ה-API של LeetCode. ייתכן שיהיה צורך לייבא `ListNode` או להניח שהפונקציות כמו `isBadVersion` מוגדרות לפי השאלה.*
