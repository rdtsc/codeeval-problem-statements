<h2>The Labyrinth</h2>

<h3>Challenge Description:</h3>

<p>
    You are given a text with a pseudographical schema of a labyrinth. Walls are marked with asterisk symbols (*). Your
    job is to write a program that finds the shortest way from the upper entrance to the lower exit and prints out
    the labyrinth schema containing a path marked with plus symbols (+).
</p>

<h3>Input sample:</h3>

<p>
    A text file with labyrinth schema.
</p>

<pre>************************* *************************
*                                   * *           *
* * *** *** ******************* ***** * * * * * ***
* * *   * *   *   * * *                 * * * *   *
***** * * *** * *** * * *** *** * ***** *** *******
*     * *   * *     *   * * *   *     * * *       *
*** ******* * ***** *** * * ******* * *** * *** * *
* *     *     *   *     *     *     * *       * * *
* * *********** * ********* * ******* * *** * *****
*     * *   * * *     *     * *   *   * *   *     *
* ***** * *** * ***** *** *** * * * ******* ***** *
* *     *   * * *       * * *   * * * *   *     * *
* * ***** *** *** *** *** * ***** *** *** ***** ***
*     *   * * *     * *       * *       * *     * *
* * ***** * * * *** * *** ***** *** ***** *** * * *
* * *           *   * *   *     *     *     * *   *
* ******* ******* * *** ******* *** * * ********* *
*   *       *     * *   *         * * * *     *   *
*** * * ***** * ***** ******* ******* * * * * * ***
*     *   *   *         *       * *   * * * * *   *
*** * *** * *** ***** ******* * * * *** *** * *** *
* * * * * * * *     * * *     *       *   * * * * *
* * *** * * * *** *** * * ********* ***** * * * * *
* * *   * * *     *   * *   *     *   *     * * * *
* * * *** ******* ***** * ******* *** * *** *** * *
* * *     *   *   *     * *     * * * *   *   * * *
* ***** * * * *** * ***** ***** * * * ***** * * * *
* *     * * * *     * *     *           * * *   * *
* ***** * *** * ***** *********** ******* * * * * *
*     * * * *             *   *     * * *   * * * *
* * * *** * *** * ***** ***** ******* * *** * * * *
* * *   * * *   *     * *             *     * * * *
* ***** * * *********** ******* *** * ******* * * *
* *     *   *   *     * *   *   * * *       * *   *
* * * ********* * ***** * *** *** *** * ***** * ***
* * *       *           *   * * *   * *   *   *   *
* ******* ***** ******* * *** * * *** *** * *******
*   *   *   *   *   *     *         * * * * * * * *
* ***** * *** ***** * ******* * ***** * *** * * * *
*     *           *     *     * * *   *   *     * *
*** *** ********************* *** *** *** *** * * *
*   *   *     *               * * *   *       *   *
*** *** * ***** * ******* *** * * *** * *** ***** *
*       *       *   *   * * *   *     *   * *   * *
*** ***** ***** *** *** *** ***** * * *** *** * * *
*       *   *   * * *       *   * * *   * *   *   *
*** *** * ***** * ***** *** *** *** *** ******* ***
*   *     *   *   *     * * * *     * * *     *   *
* ***** *** ***** ******* * * *** *** * *** ***** *
*   *                 *           *         *     *
************************* *************************</pre>

<h3>Output sample:</h3>

<p>
    Print to stdout the labyrinth schema containing the shortest way out marked with &#x2018;+&#x2019; symbols:
</p>

<pre>*************************+*************************
*                        +++++++    * *           *
* * *** *** *******************+***** * * * * * ***
* * *   * *   *   * * *    +++++        * * * *   *
***** * * *** * *** * * ***+*** * ***** *** *******
*     * *   * *     *   * *+*   *     * * *       *
*** ******* * ***** *** * *+******* * *** * *** * *
* *     *     *   *     *  +  *     * *       * * *
* * *********** * *********+* ******* * *** * *****
*     * *   * * *     *  +++* *   *   * *   *     *
* ***** * *** * ***** ***+*** * * * ******* ***** *
* *     *   * * *       *+* *   * * * *   *     * *
* * ***** *** *** *** ***+* ***** *** *** ***** ***
*     *   * * *     * *  +    * *       * *     * *
* * ***** * * * *** * ***+***** *** ***** *** * * *
* * *           *   * *+++*     *     *     * *   *
* ******* ******* * ***+******* *** * * ********* *
*   *       *     * *+++*         * * * *     *   *
*** * * ***** * *****+******* ******* * * * * * ***
*     *   *   *+++++++  *       * *   * * * * *   *
*** * *** * ***+***** ******* * * * *** *** * *** *
* * * * * * * *+++  * * *     *       *   * * * * *
* * *** * * * ***+*** * * ********* ***** * * * * *
* * *   * * *    +*   * *   *     *   *     * * * *
* * * *** *******+***** * ******* *** * *** *** * *
* * *     *   *  +*     * *     * * * *   *   * * *
* ***** * * * ***+* ***** ***** * * * ***** * * * *
* *     * * * *+++  * *     *           * * *   * *
* ***** * *** *+***** *********** ******* * * * * *
*     * * * *  +++++++++  *   *     * * *   * * * *
* * * *** * *** * *****+***** ******* * *** * * * *
* * *   * * *   *     *+*      +++++++*     * * * *
* ***** * * ***********+*******+*** *+******* * * *
* *     *   *   *     *+*   *+++* * *+      * *   *
* * * ********* * *****+* ***+*** ***+* ***** * ***
* * *       *  +++++++++*   *+* *   *+*   *   *   *
* ******* *****+******* * ***+* * ***+*** * *******
*   *   *   *+++*   *     *  +      *+* * * * * * *
* ***** * ***+***** * *******+* *****+* *** * * * *
*     *+++++++    *     *    +* * *  +*   *     * *
*** ***+*********************+*** ***+*** *** * * *
*   *  +*     *+++++++++++++++* * *  +*       *   *
*** ***+* *****+* ******* *** * * ***+* *** ***** *
*  +++++*+++++++*   *   * * *   *  +++*   * *   * *
***+*****+***** *** *** *** ***** *+* *** *** * * *
*  +++++*+  *   * * *       *   * *+*   * *   *   *
*** ***+*+***** * ***** *** *** ***+*** ******* ***
*   *  +++*   *   *     * * * *  +++* * *     *   *
* ***** *** ***** ******* * * ***+*** * *** ***** *
*   *                 *  +++++++++*         *     *
*************************+*************************</pre>

<h3>Constraints:</h3>

<p>
    The size of a labyrinth is up to 101&#xD7;101 cells. There can be more than one way to pass the labyrinth, but
    the shortest way is always unambiguous and never has branches.
</p>