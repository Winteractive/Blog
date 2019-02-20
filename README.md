# Blog
Tutorials and more

```cs
public class Progress : MonoBehaviour
{
    
    #region Variables
    public enum ProgressionStates { NewGame, Continue };
    public ProgressionStates currentState;

    public const string PROGRESS_SAVE_CODE = "PROGRESS";
    #endregion

    #region Singleton

    public static Progress INSTANCE;

    void Awake()
    {
        if (INSTANCE == null)
        {
            INSTANCE = this;
        }
        else
        {
            if (INSTANCE != this)
            {
                Destroy(this.gameObject);
            }
        }

    }

    #endregion
}
```
[![](https://pbs.twimg.com/profile_images/874988973377986561/DweZMFUi_400x400.jpg)](https://www.patreon.com/)
